# Comparing `tmp/discover-overlay-0.6.3.tar.gz` & `tmp/discover-overlay-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discover-overlay-0.6.3.tar", last modified: Thu Sep 22 12:26:14 2022, max compression
+gzip compressed data, was "discover-overlay-0.6.5.tar", last modified: Mon May 29 07:44:34 2023, max compression
```

## Comparing `discover-overlay-0.6.3.tar` & `discover-overlay-0.6.5.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:26:14.687592 discover-overlay-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4514 2022-09-22 12:26:14.687592 discover-overlay-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     5080 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover-overlay-default.png
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover-overlay-default.svg
--rw-r--r--   0 runner    (1001) docker     (121)    15132 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover-overlay-tray.png
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover-overlay-tray.svg
--rw-r--r--   0 runner    (1001) docker     (121)    15132 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover-overlay.png
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover-overlay.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:26:14.687592 discover-overlay-0.6.3/discover_overlay/
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/autostart.py
--rw-r--r--   0 runner    (1001) docker     (121)    29291 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/discord_connector.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23230 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/discover_overlay.py
--rw-r--r--   0 runner    (1001) docker     (121)     5415 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/draggable_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     6269 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/draggable_window_wayland.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:26:14.687592 discover-overlay-0.6.3/discover_overlay/glade/
--rw-r--r--   0 runner    (1001) docker     (121)   112449 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/glade/settings.glade
--rw-r--r--   0 runner    (1001) docker     (121)   112429 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/glade/settings.glade~
--rw-r--r--   0 runner    (1001) docker     (121)     7528 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/image_getter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:26:14.683592 discover-overlay-0.6.3/discover_overlay/locales/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:26:14.683592 discover-overlay-0.6.3/discover_overlay/locales/cy/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:26:14.687592 discover-overlay-0.6.3/discover_overlay/locales/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     6968 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/locales/cy/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:26:14.683592 discover-overlay-0.6.3/discover_overlay/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:26:14.687592 discover-overlay-0.6.3/discover_overlay/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/locales/en/LC_MESSAGES/default.mo
--rw-r--r--   0 runner    (1001) docker     (121)    19142 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/notification_overlay.py
--rw-r--r--   0 runner    (1001) docker     (121)    11945 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/overlay.py
--rw-r--r--   0 runner    (1001) docker     (121)    43480 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/settings_window.py
--rw-r--r--   0 runner    (1001) docker     (121)    13205 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/text_overlay.py
--rw-r--r--   0 runner    (1001) docker     (121)    37411 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay/voice_overlay.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay.desktop
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:26:14.687592 discover-overlay-0.6.3/discover_overlay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4514 2022-09-22 12:26:14.000000 discover-overlay-0.6.3/discover_overlay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-09-22 12:26:14.000000 discover-overlay-0.6.3/discover_overlay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 12:26:14.000000 discover-overlay-0.6.3/discover_overlay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-22 12:26:14.000000 discover-overlay-0.6.3/discover_overlay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-22 12:26:14.000000 discover-overlay-0.6.3/discover_overlay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-22 12:26:14.000000 discover-overlay-0.6.3/discover_overlay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/discover_overlay_configure.desktop
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 12:26:14.687592 discover-overlay-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-09-22 12:26:06.000000 discover-overlay-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.526143 discover-overlay-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-29 07:44:34.526143 discover-overlay-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover-overlay-default.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover-overlay-default.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15132 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover-overlay-tray.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover-overlay-tray.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15132 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover-overlay.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover-overlay.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.522143 discover-overlay-0.6.5/discover_overlay/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/discord_connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23459 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/discover_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/draggable_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/draggable_window_wayland.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.526143 discover-overlay-0.6.5/discover_overlay/glade/
+-rw-r--r--   0 runner    (1001) docker     (123)   118691 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/glade/settings.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/image_getter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.518143 discover-overlay-0.6.5/discover_overlay/locales/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.518143 discover-overlay-0.6.5/discover_overlay/locales/cy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.526143 discover-overlay-0.6.5/discover_overlay/locales/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/locales/cy/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.518143 discover-overlay-0.6.5/discover_overlay/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.526143 discover-overlay-0.6.5/discover_overlay/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/locales/de/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.518143 discover-overlay-0.6.5/discover_overlay/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.526143 discover-overlay-0.6.5/discover_overlay/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/locales/en/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.518143 discover-overlay-0.6.5/discover_overlay/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.526143 discover-overlay-0.6.5/discover_overlay/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/locales/tr/LC_MESSAGES/default.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/notification_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46114 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/settings_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/text_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39156 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay/voice_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:44:34.526143 discover-overlay-0.6.5/discover_overlay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-29 07:44:34.000000 discover-overlay-0.6.5/discover_overlay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-29 07:44:34.000000 discover-overlay-0.6.5/discover_overlay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:44:34.000000 discover-overlay-0.6.5/discover_overlay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-29 07:44:34.000000 discover-overlay-0.6.5/discover_overlay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 07:44:34.000000 discover-overlay-0.6.5/discover_overlay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 07:44:34.000000 discover-overlay-0.6.5/discover_overlay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/discover_overlay_configure.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 07:44:34.526143 discover-overlay-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-29 07:44:24.000000 discover-overlay-0.6.5/setup.py
```

### Comparing `discover-overlay-0.6.3/LICENSE` & `discover-overlay-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/PKG-INFO` & `discover-overlay-0.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discover-overlay
-Version: 0.6.3
+Version: 0.6.5
 Summary: Voice chat overlay
 Home-page: https://github.com/trigg/Discover
 Author: trigg
 Author-email: 
 License: GPLv3+
 Keywords: discord overlay voice linux
 Classifier: Development Status :: 4 - Beta
@@ -85,19 +85,21 @@
 
 A compositor is strongly advised but there is a non-compositor mode optionally
 
 It is advised to install python-gobject from your system's own package manager.
 
 #### Debian/Ubuntu
 
-`apt install python3-gi python3-gi-cairo`
+`apt install python3-gi python3-gi-cairo libappindicator3-dev`
+
+Libappindicator might conflict with other installed packages, but is optional
 
 with Wayland support
 
-`apt install gtk-layer-shell`
+`apt install gtk-layer-shell libgtk-layer-shell-dev`
 
 #### Arch
 
 `pacman -S python-gobject libappindicator-gtk3`
 
 with Wayland support
```

### Comparing `discover-overlay-0.6.3/README.md` & `discover-overlay-0.6.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -65,19 +65,21 @@
 
 A compositor is strongly advised but there is a non-compositor mode optionally
 
 It is advised to install python-gobject from your system's own package manager.
 
 #### Debian/Ubuntu
 
-`apt install python3-gi python3-gi-cairo`
+`apt install python3-gi python3-gi-cairo libappindicator3-dev`
+
+Libappindicator might conflict with other installed packages, but is optional
 
 with Wayland support
 
-`apt install gtk-layer-shell`
+`apt install gtk-layer-shell libgtk-layer-shell-dev`
 
 #### Arch
 
 `pacman -S python-gobject libappindicator-gtk3`
 
 with Wayland support
```

### Comparing `discover-overlay-0.6.3/discover-overlay-default.png` & `discover-overlay-0.6.5/discover-overlay-default.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover-overlay-default.svg` & `discover-overlay-0.6.5/discover-overlay-default.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover-overlay-tray.png` & `discover-overlay-0.6.5/discover-overlay-tray.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover-overlay-tray.svg` & `discover-overlay-0.6.5/discover-overlay-tray.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover-overlay.png` & `discover-overlay-0.6.5/discover-overlay.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover-overlay.svg` & `discover-overlay-0.6.5/discover-overlay.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover_overlay/__init__.py` & `discover-overlay-0.6.5/discover_overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover_overlay/__main__.py` & `discover-overlay-0.6.5/discover_overlay/__main__.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover_overlay/autostart.py` & `discover-overlay-0.6.5/discover_overlay/autostart.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover_overlay/discord_connector.py` & `discover-overlay-0.6.5/discover_overlay/discord_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -753,15 +753,15 @@
                 # Receive & send to on_message
                 msg = self.websocket.recv()
                 self.on_message(msg)
                 if not self.websocket:
                     # Connection was closed in the meantime
                     return True
                 recv, _w, _e = select.select((self.websocket.sock,), (), (), 0)
-            except websocket.WebSocketConnectionClosedException:
+            except (websocket.WebSocketConnectionClosedException, json.decoder.JSONDecodeError):
                 self.on_close()
                 return True
         return True
 
     def start_listening_text(self, channel):
         """
         Subscribe to text events on channel, or remember the channel for when we've connected
```

### Comparing `discover-overlay-0.6.3/discover_overlay/discover_overlay.py` & `discover-overlay-0.6.5/discover_overlay/discover_overlay.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,16 @@
             "main", "text_baseline_adj", fallback=0))
         font = config.get("main", "font", fallback=None)
         title_font = config.get("main", "title_font", fallback=None)
         self.voice_overlay.set_square_avatar(config.getboolean(
             "main", "square_avatar", fallback=True))
         self.voice_overlay.set_only_speaking(config.getboolean(
             "main", "only_speaking", fallback=False))
+        self.voice_overlay.set_only_speaking_grace_period(config.getint(
+            "main", "only_speaking_grace", fallback=0))
         self.voice_overlay.set_highlight_self(config.getboolean(
             "main", "highlight_self", fallback=False))
         self.voice_overlay.set_icon_only(config.getboolean(
             "main", "icon_only", fallback=False))
         monitor = config.get("main", "monitor", fallback="None")
         self.voice_overlay.set_vert_edge_padding(config.getint(
             "main", "vert_edge_padding", fallback=0))
@@ -266,14 +268,15 @@
             "main", "show_title", fallback=False))
         self.voice_overlay.set_show_disconnected(config.getboolean(
             "main", "show_disconnected", fallback=False))
         self.voice_overlay.set_border_width(
             config.getint("main", "border_width", fallback=2))
         self.voice_overlay.set_icon_transparency(config.getfloat(
             "main", "icon_transparency", fallback=1.0))
+        self.voice_overlay.set_show_avatar(config.getboolean("main", "show_avatar", fallback=True))
         self.voice_overlay.set_fancy_border(config.getboolean("main",
                                                               "fancy_border", fallback=True))
         self.voice_overlay.set_show_dummy(config.getboolean("main",
                                                             "show_dummy", fallback=False))
         self.voice_overlay.set_dummy_count(config.getint("main",
                                                          "dummy_count", fallback=10))
```

### Comparing `discover-overlay-0.6.3/discover_overlay/draggable_window.py` & `discover-overlay-0.6.5/discover_overlay/draggable_window.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover_overlay/draggable_window_wayland.py` & `discover-overlay-0.6.5/discover_overlay/draggable_window_wayland.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover_overlay/glade/settings.glade` & `discover-overlay-0.6.5/discover_overlay/glade/settings.glade`

 * *Files 1% similar despite different names*

#### Comparing `discover-overlay-0.6.3/discover_overlay/glade/settings.glade` & `discover-overlay-0.6.5/discover_overlay/glade/settings.glade`

```diff
@@ -106,28 +106,40 @@
     <property name="page-increment">10</property>
   </object>
   <object class="GtkAdjustment" id="text_padding_adj">
     <property name="upper">64</property>
     <property name="step-increment">1</property>
     <property name="page-increment">1</property>
   </object>
+  <object class="GtkAdjustment" id="text_popup_time_adj">
+    <property name="lower">30</property>
+    <property name="upper">5000</property>
+    <property name="value">30</property>
+    <property name="step-increment">1</property>
+    <property name="page-increment">10</property>
+  </object>
   <object class="GtkListStore" id="voice_align_1_list">
     <columns>
       <!-- column-name key -->
       <column type="gchararray"/>
     </columns>
     <data>
       <row>
         <col id="0" translatable="yes">Left</col>
       </row>
       <row>
         <col id="0" translatable="yes">Right</col>
       </row>
     </data>
   </object>
+  <object class="GtkAdjustment" id="voice_display_speakers_grace_period_adj">
+    <property name="upper">360</property>
+    <property name="step-increment">1</property>
+    <property name="page-increment">10</property>
+  </object>
   <object class="GtkAdjustment" id="voice_dummy_count_adj">
     <property name="lower">10</property>
     <property name="upper">100</property>
     <property name="value">50</property>
     <property name="step-increment">1</property>
     <property name="page-increment">10</property>
   </object>
@@ -690,650 +702,741 @@
               </object>
               <packing>
                 <property name="left-attach">1</property>
                 <property name="top-attach">0</property>
               </packing>
             </child>
             <child>
-              <!-- n-columns=6 n-rows=8 -->
+              <!-- n-columns=6 n-rows=10 -->
               <object class="GtkGrid">
                 <property name="name">voice_advanced_grid</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
                 <property name="row-spacing">1</property>
                 <property name="column-spacing">5</property>
                 <property name="column-homogeneous">True</property>
                 <child>
-                  <object class="GtkFontButton">
-                    <property name="name">voice_font</property>
+                  <object class="GtkLabel">
+                    <property name="name">voice_display_icon_only_label</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">False</property>
+                    <property name="label" translatable="yes">Show Names</property>
+                    <property name="xalign">0</property>
+                  </object>
+                  <packing>
+                    <property name="left-attach">2</property>
+                    <property name="top-attach">0</property>
+                  </packing>
+                </child>
+                <child>
+                  <object class="GtkCheckButton">
+                    <property name="name">voice_display_icon_only</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="font">Sans 12</property>
-                    <property name="language">en-us</property>
-                    <property name="preview-text"/>
-                    <signal name="font-set" handler="voice_font_changed" swapped="no"/>
+                    <property name="receives-default">False</property>
+                    <property name="draw-indicator">True</property>
+                    <signal name="toggled" handler="voice_display_icon_only_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">1</property>
+                    <property name="left-attach">3</property>
                     <property name="top-attach">0</property>
                   </packing>
                 </child>
                 <child>
+                  <object class="GtkLabel">
+                    <property name="name">voice_font_label</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">False</property>
+                    <property name="label" translatable="yes">Font</property>
+                    <property name="xalign">0</property>
+                  </object>
+                  <packing>
+                    <property name="left-attach">2</property>
+                    <property name="top-attach">1</property>
+                  </packing>
+                </child>
+                <child>
                   <object class="GtkFontButton">
-                    <property name="name">voice_title_font</property>
+                    <property name="name">voice_font</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
                     <property name="receives-default">True</property>
                     <property name="font">Sans 12</property>
                     <property name="language">en-us</property>
                     <property name="preview-text"/>
-                    <signal name="font-set" handler="voice_title_font_changed" swapped="no"/>
+                    <signal name="font-set" handler="voice_font_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">1</property>
+                    <property name="left-attach">3</property>
                     <property name="top-attach">1</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_font_label</property>
+                    <property name="name">voice_text_padding_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Font</property>
+                    <property name="label" translatable="yes">Text Padding</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">0</property>
+                    <property name="left-attach">2</property>
+                    <property name="top-attach">2</property>
+                  </packing>
+                </child>
+                <child>
+                  <object class="GtkSpinButton">
+                    <property name="name">voice_text_padding</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">True</property>
+                    <property name="text" translatable="yes">0</property>
+                    <property name="adjustment">text_padding_adj</property>
+                    <signal name="value-changed" handler="voice_text_padding_changed" swapped="no"/>
+                  </object>
+                  <packing>
+                    <property name="left-attach">3</property>
+                    <property name="top-attach">2</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_title_font_label</property>
+                    <property name="name">voice_text_vertical_offset_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Title Font</property>
+                    <property name="label" translatable="yes">Text Vertical Offset</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">1</property>
+                    <property name="left-attach">2</property>
+                    <property name="top-attach">3</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkSpinButton">
-                    <property name="name">voice_icon_spacing</property>
+                    <property name="name">voice_text_vertical_offset</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="adjustment">icon_spacing_adj</property>
-                    <signal name="value-changed" handler="voice_icon_spacing_changed" swapped="no"/>
+                    <property name="text" translatable="yes">0</property>
+                    <property name="adjustment">voice_text_offset</property>
+                    <signal name="value-changed" handler="voice_text_vertical_offset_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">2</property>
+                    <property name="left-attach">3</property>
+                    <property name="top-attach">3</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_icon_spacing_label</property>
+                    <property name="name">voice_show_title_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Icon Spacing</property>
+                    <property name="label" translatable="yes">Show Title</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
                     <property name="left-attach">0</property>
-                    <property name="top-attach">2</property>
+                    <property name="top-attach">0</property>
+                  </packing>
+                </child>
+                <child>
+                  <object class="GtkCheckButton">
+                    <property name="name">voice_show_title</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">True</property>
+                    <property name="receives-default">False</property>
+                    <property name="draw-indicator">True</property>
+                    <signal name="toggled" handler="voice_show_title_changed" swapped="no"/>
+                  </object>
+                  <packing>
+                    <property name="left-attach">1</property>
+                    <property name="top-attach">0</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_text_padding_label</property>
+                    <property name="name">voice_show_connection_status_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Text Padding</property>
+                    <property name="label" translatable="yes">Show Connection Status</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
                     <property name="left-attach">0</property>
-                    <property name="top-attach">3</property>
+                    <property name="top-attach">2</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_text_padding</property>
+                  <object class="GtkCheckButton">
+                    <property name="name">voice_show_connection_status</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="adjustment">text_padding_adj</property>
-                    <signal name="value-changed" handler="voice_text_padding_changed" swapped="no"/>
+                    <property name="receives-default">False</property>
+                    <property name="draw-indicator">True</property>
+                    <signal name="toggled" handler="voice_show_connection_status_changed" swapped="no"/>
                   </object>
                   <packing>
                     <property name="left-attach">1</property>
-                    <property name="top-attach">3</property>
+                    <property name="top-attach">2</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_text_vertical_offset_label</property>
+                  <object class="GtkFontButton">
+                    <property name="name">voice_title_font</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Text Vertical Offset</property>
-                    <property name="xalign">0</property>
+                    <property name="can-focus">True</property>
+                    <property name="receives-default">True</property>
+                    <property name="font">Sans 12</property>
+                    <property name="language">en-us</property>
+                    <property name="preview-text"/>
+                    <signal name="font-set" handler="voice_title_font_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">4</property>
+                    <property name="left-attach">1</property>
+                    <property name="top-attach">1</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voce_vertical_padding_label</property>
+                    <property name="name">voice_title_font_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Verticle Edge Padding</property>
+                    <property name="label" translatable="yes">Title Font</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
                     <property name="left-attach">0</property>
-                    <property name="top-attach">5</property>
+                    <property name="top-attach">1</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_horizontal_padding_label</property>
+                  <object class="GtkSpinButton">
+                    <property name="name">voice_vertical_padding</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Horizontal Edge Padding</property>
-                    <property name="xalign">0</property>
+                    <property name="can-focus">True</property>
+                    <property name="text" translatable="yes">0</property>
+                    <property name="adjustment">voice_vertical_padding_adj</property>
+                    <signal name="value-changed" handler="voice_vertical_padding_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">6</property>
+                    <property name="left-attach">1</property>
+                    <property name="top-attach">4</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_avatar_opacity_label</property>
+                    <property name="name">voice_horizontal_padding_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Avatar Opacity</property>
+                    <property name="label" translatable="yes">Horizontal Edge Padding</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">0</property>
+                    <property name="left-attach">0</property>
+                    <property name="top-attach">5</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_avatar_size_label</property>
+                  <object class="GtkSpinButton">
+                    <property name="name">voice_horizontal_padding</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Avatar Size</property>
-                    <property name="xalign">0</property>
+                    <property name="can-focus">True</property>
+                    <property name="text" translatable="yes">0</property>
+                    <property name="adjustment">voice_horizontal_padding_adj</property>
+                    <signal name="value-changed" handler="voice_horizontal_padding_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">1</property>
+                    <property name="left-attach">1</property>
+                    <property name="top-attach">5</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_display_icon_only_label</property>
+                    <property name="name">voice_show_test_content_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Display Icon Only</property>
+                    <property name="label" translatable="yes">Show Test Content</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">2</property>
+                    <property name="left-attach">0</property>
+                    <property name="top-attach">7</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_square_avatar_label</property>
+                  <object class="GtkCheckButton">
+                    <property name="name">voice_show_test_content</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Square Avatar</property>
-                    <property name="xalign">0</property>
+                    <property name="can-focus">True</property>
+                    <property name="receives-default">False</property>
+                    <property name="draw-indicator">True</property>
+                    <signal name="toggled" handler="voice_toggle_test_content" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">3</property>
+                    <property name="left-attach">1</property>
+                    <property name="top-attach">7</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_fancy_avatar_shapes_label</property>
+                    <property name="name">voice_dummy_count_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Fancy Avatar Shapes</property>
+                    <property name="label" translatable="yes">Test Data Count</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">4</property>
+                    <property name="left-attach">0</property>
+                    <property name="top-attach">8</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkScale">
-                    <property name="name">voice_avatar_opacity</property>
+                  <object class="GtkSpinButton">
+                    <property name="name">voice_dummy_count</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="adjustment">ava_opacity_adj</property>
-                    <property name="round-digits">1</property>
-                    <signal name="value-changed" handler="voice_avatar_opacity_changed" swapped="no"/>
+                    <property name="text" translatable="yes">50</property>
+                    <property name="adjustment">voice_dummy_count_adj</property>
+                    <property name="value">50</property>
+                    <signal name="value-changed" handler="voice_dummy_count_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">0</property>
+                    <property name="left-attach">1</property>
+                    <property name="top-attach">8</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_avatar_size</property>
+                  <object class="GtkLabel">
+                    <property name="name">voice_show_disconnected_label</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="adjustment">avatar_size_adj</property>
-                    <signal name="value-changed" handler="voice_avatar_size_changed" swapped="no"/>
+                    <property name="can-focus">False</property>
+                    <property name="label" translatable="yes">Show While Disconnected</property>
+                    <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">1</property>
+                    <property name="left-attach">0</property>
+                    <property name="top-attach">9</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkCheckButton">
-                    <property name="name">voice_display_icon_only</property>
+                    <property name="name">voice_show_disconnected</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
                     <property name="receives-default">False</property>
                     <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_display_icon_only_changed" swapped="no"/>
+                    <signal name="toggled" handler="voice_show_disconnected_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">2</property>
+                    <property name="left-attach">1</property>
+                    <property name="top-attach">9</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_square_avatar</property>
+                  <object class="GtkLabel">
+                    <property name="name">voce_vertical_padding_label</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_square_avatar_changed" swapped="no"/>
+                    <property name="can-focus">False</property>
+                    <property name="label" translatable="yes">Verticle Edge Padding</property>
+                    <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">3</property>
+                    <property name="left-attach">0</property>
+                    <property name="top-attach">4</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_fancy_avatar_shapes</property>
+                  <object class="GtkLabel">
+                    <property name="name">voice_nick_length_label</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_fancy_avatar_shapes_changed" swapped="no"/>
+                    <property name="can-focus">False</property>
+                    <property name="label" translatable="yes">Limit text length</property>
+                    <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">3</property>
+                    <property name="left-attach">2</property>
                     <property name="top-attach">4</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkSpinButton">
-                    <property name="name">voice_horizontal_padding</property>
+                    <property name="name">voice_nick_length</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="adjustment">voice_horizontal_padding_adj</property>
-                    <signal name="value-changed" handler="voice_horizontal_padding_changed" swapped="no"/>
+                    <property name="text" translatable="yes">32</property>
+                    <property name="adjustment">voice_nick_lenght_adj</property>
+                    <property name="value">32</property>
+                    <signal name="value-changed" handler="voice_nick_length_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">6</property>
+                    <property name="left-attach">3</property>
+                    <property name="top-attach">4</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_vertical_padding</property>
+                  <object class="GtkLabel">
+                    <property name="name">voice_avatar_label</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="adjustment">voice_vertical_padding_adj</property>
-                    <signal name="value-changed" handler="voice_vertical_padding_changed" swapped="no"/>
+                    <property name="can-focus">False</property>
+                    <property name="label" translatable="yes">Show Avatar</property>
+                    <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">1</property>
+                    <property name="left-attach">2</property>
                     <property name="top-attach">5</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_text_vertical_offset</property>
+                  <object class="GtkCheckButton">
+                    <property name="name">voice_show_avatar</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="adjustment">voice_text_offset</property>
-                    <signal name="value-changed" handler="voice_text_vertical_offset_changed" swapped="no"/>
+                    <property name="receives-default">False</property>
+                    <property name="draw-indicator">True</property>
+                    <signal name="toggled" handler="voice_show_avatar_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">4</property>
+                    <property name="left-attach">3</property>
+                    <property name="top-attach">5</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_overflow_style_label</property>
+                    <property name="name">voice_square_avatar_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Overflow Style</property>
+                    <property name="label" translatable="yes">Square Avatar</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">0</property>
+                    <property name="left-attach">2</property>
+                    <property name="top-attach">6</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkComboBoxText" id="voice_overflow_style">
-                    <property name="name">voice_overflow_style</property>
+                  <object class="GtkCheckButton">
+                    <property name="name">voice_square_avatar</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <items>
-                      <item translatable="yes">None</item>
-                      <item translatable="yes">Wrap</item>
-                      <item translatable="yes">Shrink</item>
-                    </items>
-                    <signal name="changed" handler="voice_overflow_style_changed" swapped="no"/>
+                    <property name="can-focus">True</property>
+                    <property name="receives-default">False</property>
+                    <property name="draw-indicator">True</property>
+                    <signal name="toggled" handler="voice_square_avatar_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">0</property>
+                    <property name="left-attach">3</property>
+                    <property name="top-attach">6</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_order_avatars_by_label</property>
+                    <property name="name">voice_fancy_avatar_shapes_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Order Avatars By</property>
+                    <property name="label" translatable="yes">Fancy Avatar Shapes</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">1</property>
+                    <property name="left-attach">2</property>
+                    <property name="top-attach">7</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkComboBoxText" id="voice_order_avatars_by">
-                    <property name="name">voice_order_avatars_by</property>
+                  <object class="GtkCheckButton">
+                    <property name="name">voice_fancy_avatar_shapes</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <items>
-                      <item translatable="yes">Alphabetically</item>
-                      <item translatable="yes">ID</item>
-                      <item translatable="yes">Last Spoken</item>
-                    </items>
-                    <signal name="changed" handler="voice_order_avatars_by_changed" swapped="no"/>
+                    <property name="can-focus">True</property>
+                    <property name="receives-default">False</property>
+                    <property name="draw-indicator">True</property>
+                    <signal name="toggled" handler="voice_fancy_avatar_shapes_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">1</property>
+                    <property name="left-attach">3</property>
+                    <property name="top-attach">7</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_border_width_label</property>
+                    <property name="name">voice_avatar_size_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Border width</property>
+                    <property name="label" translatable="yes">Avatar Size</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
                     <property name="left-attach">2</property>
-                    <property name="top-attach">5</property>
+                    <property name="top-attach">8</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkSpinButton">
-                    <property name="name">voice_border_width</property>
+                    <property name="name">voice_avatar_size</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="adjustment">border_width_adj</property>
-                    <signal name="value-changed" handler="voice_border_width_changed" swapped="no"/>
+                    <property name="text" translatable="yes">48</property>
+                    <property name="adjustment">avatar_size_adj</property>
+                    <property name="value">48</property>
+                    <signal name="value-changed" handler="voice_avatar_size_changed" swapped="no"/>
                   </object>
                   <packing>
                     <property name="left-attach">3</property>
-                    <property name="top-attach">5</property>
+                    <property name="top-attach">8</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_show_title_label</property>
+                    <property name="name">voice_avatar_opacity_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show Title</property>
+                    <property name="label" translatable="yes">Avatar Opacity</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">2</property>
+                    <property name="left-attach">2</property>
+                    <property name="top-attach">9</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_show_title</property>
+                  <object class="GtkScale">
+                    <property name="name">voice_avatar_opacity</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_show_title_changed" swapped="no"/>
+                    <property name="adjustment">ava_opacity_adj</property>
+                    <property name="round-digits">1</property>
+                    <signal name="value-changed" handler="voice_avatar_opacity_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">2</property>
+                    <property name="left-attach">3</property>
+                    <property name="top-attach">9</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_show_connection_status_label</property>
+                    <property name="name">voice_display_speakers_only_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show Connection Status</property>
+                    <property name="label" translatable="yes">Display Speakers Only</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
                     <property name="left-attach">4</property>
-                    <property name="top-attach">3</property>
+                    <property name="top-attach">0</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkCheckButton">
-                    <property name="name">voice_show_connection_status</property>
+                    <property name="name">voice_display_speakers_only</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
                     <property name="receives-default">False</property>
                     <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_show_connection_status_changed" swapped="no"/>
+                    <signal name="toggled" handler="voice_display_speakers_only" swapped="no"/>
                   </object>
                   <packing>
                     <property name="left-attach">5</property>
-                    <property name="top-attach">3</property>
+                    <property name="top-attach">0</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_show_disconnected_label</property>
+                    <property name="name">voice_display_speakers_grace_period_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show While Disconnected</property>
+                    <property name="label" translatable="yes">Speakers Grace Period</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
                     <property name="left-attach">4</property>
-                    <property name="top-attach">4</property>
+                    <property name="top-attach">1</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_show_disconnected</property>
+                  <object class="GtkSpinButton">
+                    <property name="name">voice_display_speakers_grace_period</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_show_disconnected_changed" swapped="no"/>
+                    <property name="text" translatable="yes">0</property>
+                    <property name="adjustment">voice_display_speakers_grace_period_adj</property>
+                    <signal name="value-changed" handler="voice_display_speakers_grace_period" swapped="no"/>
                   </object>
                   <packing>
                     <property name="left-attach">5</property>
-                    <property name="top-attach">4</property>
+                    <property name="top-attach">1</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_highlight_self_label</property>
+                    <property name="name">voice_overflow_style_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Highlight Self</property>
+                    <property name="label" translatable="yes">Overflow Style</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">6</property>
+                    <property name="left-attach">4</property>
+                    <property name="top-attach">2</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_highlight_self</property>
+                  <object class="GtkComboBoxText" id="voice_overflow_style">
+                    <property name="name">voice_overflow_style</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_highlight_self_changed" swapped="no"/>
+                    <property name="can-focus">False</property>
+                    <items>
+                      <item translatable="yes">None</item>
+                      <item translatable="yes">Wrap</item>
+                      <item translatable="yes">Shrink</item>
+                    </items>
+                    <signal name="changed" handler="voice_overflow_style_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">6</property>
+                    <property name="left-attach">5</property>
+                    <property name="top-attach">2</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_show_test_content_label</property>
+                    <property name="name">voice_order_avatars_by_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show Test Content</property>
+                    <property name="label" translatable="yes">Order Users By</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">7</property>
+                    <property name="left-attach">4</property>
+                    <property name="top-attach">3</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_show_test_content</property>
+                  <object class="GtkComboBoxText" id="voice_order_avatars_by">
+                    <property name="name">voice_order_avatars_by</property>
                     <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_toggle_test_content" swapped="no"/>
+                    <property name="can-focus">False</property>
+                    <items>
+                      <item translatable="yes">Alphabetically</item>
+                      <item translatable="yes">ID</item>
+                      <item translatable="yes">Last Spoken</item>
+                    </items>
+                    <signal name="changed" handler="voice_order_avatars_by_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">7</property>
+                    <property name="left-attach">5</property>
+                    <property name="top-attach">3</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_dummy_count_label</property>
+                    <property name="name">voice_highlight_self_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Dummy Count</property>
+                    <property name="label" translatable="yes">Highlight Self</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">7</property>
+                    <property name="left-attach">4</property>
+                    <property name="top-attach">4</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_dummy_count</property>
+                  <object class="GtkCheckButton">
+                    <property name="name">voice_highlight_self</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="adjustment">voice_dummy_count_adj</property>
-                    <signal name="value-changed" handler="voice_dummy_count_changed" swapped="no"/>
+                    <property name="receives-default">False</property>
+                    <property name="draw-indicator">True</property>
+                    <signal name="toggled" handler="voice_highlight_self_changed" swapped="no"/>
                   </object>
                   <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">7</property>
+                    <property name="left-attach">5</property>
+                    <property name="top-attach">4</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_display_speakers_only_label</property>
+                    <property name="name">voice_border_width_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Display Speakers Only</property>
+                    <property name="label" translatable="yes">Border width</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
                     <property name="left-attach">4</property>
                     <property name="top-attach">5</property>
                   </packing>
                 </child>
                 <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_display_speakers_only</property>
+                  <object class="GtkSpinButton">
+                    <property name="name">voice_border_width</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_display_speakers_only" swapped="no"/>
+                    <property name="text" translatable="yes">1</property>
+                    <property name="adjustment">border_width_adj</property>
+                    <property name="value">1</property>
+                    <signal name="value-changed" handler="voice_border_width_changed" swapped="no"/>
                   </object>
                   <packing>
                     <property name="left-attach">5</property>
                     <property name="top-attach">5</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkLabel">
-                    <property name="name">voice_nick_length_label</property>
+                    <property name="name">voice_icon_spacing_label</property>
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Limit text length</property>
+                    <property name="label" translatable="yes">Padding between users</property>
                     <property name="xalign">0</property>
                   </object>
                   <packing>
                     <property name="left-attach">4</property>
                     <property name="top-attach">6</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkSpinButton">
-                    <property name="name">voice_nick_length</property>
+                    <property name="name">voice_icon_spacing</property>
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
-                    <property name="adjustment">voice_nick_lenght_adj</property>
-                    <signal name="value-changed" handler="voice_nick_length_changed" swapped="no"/>
+                    <property name="text" translatable="yes">0</property>
+                    <property name="adjustment">icon_spacing_adj</property>
+                    <signal name="value-changed" handler="voice_icon_spacing_changed" swapped="no"/>
                   </object>
                   <packing>
                     <property name="left-attach">5</property>
                     <property name="top-attach">6</property>
                   </packing>
                 </child>
                 <child>
                   <placeholder/>
                 </child>
                 <child>
                   <placeholder/>
                 </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
               </object>
               <packing>
                 <property name="left-attach">0</property>
                 <property name="top-attach">1</property>
                 <property name="width">2</property>
               </packing>
             </child>
@@ -1351,15 +1454,15 @@
           </object>
           <packing>
             <property name="position">1</property>
             <property name="tab-fill">False</property>
           </packing>
         </child>
         <child>
-          <!-- n-columns=2 n-rows=12 -->
+          <!-- n-columns=2 n-rows=13 -->
           <object class="GtkGrid">
             <property name="name">text_grid</property>
             <property name="visible">True</property>
             <property name="can-focus">False</property>
             <property name="margin-start">5</property>
             <property name="margin-end">5</property>
             <property name="margin-top">5</property>
@@ -1419,83 +1522,73 @@
               <packing>
                 <property name="left-attach">1</property>
                 <property name="top-attach">1</property>
               </packing>
             </child>
             <child>
               <object class="GtkLabel">
-                <property name="name">text_server_label</property>
+                <property name="name">text_line_limit_label</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
-                <property name="label" translatable="yes">Server</property>
+                <property name="label" translatable="yes">Line Limit</property>
                 <property name="xalign">0</property>
               </object>
               <packing>
                 <property name="left-attach">0</property>
-                <property name="top-attach">2</property>
+                <property name="top-attach">12</property>
               </packing>
             </child>
             <child>
-              <object class="GtkComboBoxText">
-                <property name="name">text_server</property>
+              <object class="GtkSpinButton">
+                <property name="name">text_line_limit</property>
                 <property name="visible">True</property>
-                <property name="can-focus">False</property>
+                <property name="can-focus">True</property>
+                <property name="text" translatable="yes">10</property>
+                <property name="adjustment">text_line_limit_adj</property>
+                <property name="value">10</property>
+                <signal name="value-changed" handler="text_line_limit_changed" swapped="no"/>
               </object>
               <packing>
                 <property name="left-attach">1</property>
-                <property name="top-attach">2</property>
+                <property name="top-attach">12</property>
               </packing>
             </child>
             <child>
               <object class="GtkLabel">
-                <property name="name">text_line_limit_label</property>
+                <property name="name">text_show_attachments_label</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
-                <property name="label" translatable="yes">Line Limit</property>
+                <property name="label" translatable="yes">Show Attachments</property>
                 <property name="xalign">0</property>
               </object>
               <packing>
                 <property name="left-attach">0</property>
                 <property name="top-attach">11</property>
               </packing>
             </child>
             <child>
-              <object class="GtkSpinButton">
-                <property name="name">text_line_limit</property>
-                <property name="visible">True</property>
-                <property name="can-focus">True</property>
-                <property name="adjustment">text_line_limit_adj</property>
-                <property name="value">10</property>
-                <signal name="value-changed" handler="text_line_limit_changed" swapped="no"/>
-              </object>
-              <packing>
-                <property name="left-attach">1</property>
-                <property name="top-attach">11</property>
-              </packing>
-            </child>
-            <child>
               <object class="GtkCheckButton">
                 <property name="name">text_show_attachments</property>
                 <property name="visible">True</property>
                 <property name="can-focus">True</property>
                 <property name="receives-default">False</property>
                 <property name="draw-indicator">True</property>
                 <signal name="toggled" handler="text_show_attachments_changed" swapped="no"/>
               </object>
               <packing>
                 <property name="left-attach">1</property>
-                <property name="top-attach">10</property>
+                <property name="top-attach">11</property>
               </packing>
             </child>
             <child>
               <object class="GtkLabel">
-                <property name="name">text_show_attachments_label</property>
+                <property name="name">text_overlay_location_label</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
-                <property name="label" translatable="yes">Show Attachments</property>
+                <property name="label" translatable="yes">Overlay Location</property>
                 <property name="xalign">0</property>
               </object>
               <packing>
                 <property name="left-attach">0</property>
                 <property name="top-attach">10</property>
               </packing>
             </child>
@@ -1506,167 +1599,206 @@
                 <property name="visible">True</property>
                 <property name="can-focus">True</property>
                 <property name="receives-default">True</property>
                 <signal name="pressed" handler="text_place_window" swapped="no"/>
               </object>
               <packing>
                 <property name="left-attach">1</property>
-                <property name="top-attach">9</property>
+                <property name="top-attach">10</property>
               </packing>
             </child>
             <child>
-              <object class="GtkLabel">
-                <property name="name">text_overlay_location_label</property>
+              <object class="GtkComboBoxText">
+                <property name="name">text_monitor</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
-                <property name="label" translatable="yes">Overlay Location</property>
-                <property name="xalign">0</property>
+                <signal name="changed" handler="text_monitor_changed" swapped="no"/>
               </object>
               <packing>
-                <property name="left-attach">0</property>
-                <property name="top-attach">8</property>
-                <property name="height">2</property>
+                <property name="left-attach">1</property>
+                <property name="top-attach">9</property>
               </packing>
             </child>
             <child>
-              <object class="GtkComboBoxText">
-                <property name="name">text_monitor</property>
+              <object class="GtkLabel">
+                <property name="name">text_background_colour_label</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
-                <signal name="changed" handler="text_monitor_changed" swapped="no"/>
+                <property name="label" translatable="yes">Background Colour</property>
+                <property name="xalign">0</property>
               </object>
               <packing>
-                <property name="left-attach">1</property>
+                <property name="left-attach">0</property>
                 <property name="top-attach">8</property>
               </packing>
             </child>
             <child>
               <object class="GtkColorButton">
                 <property name="name">text_background_colour</property>
                 <property name="visible">True</property>
                 <property name="can-focus">True</property>
                 <property name="receives-default">True</property>
                 <property name="use-alpha">True</property>
                 <signal name="color-set" handler="text_background_colour_changed" swapped="no"/>
               </object>
               <packing>
                 <property name="left-attach">1</property>
+                <property name="top-attach">8</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">text_colour_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Text Colour</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
                 <property name="top-attach">7</property>
               </packing>
             </child>
             <child>
               <object class="GtkColorButton">
                 <property name="name">text_colour</property>
                 <property name="visible">True</property>
                 <property name="can-focus">True</property>
                 <property name="receives-default">True</property>
                 <property name="use-alpha">True</property>
                 <signal name="color-set" handler="text_colour_changed" swapped="no"/>
               </object>
               <packing>
                 <property name="left-attach">1</property>
+                <property name="top-attach">7</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkFontButton">
+                <property name="name">text_font</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="font">Sans 12</property>
+                <property name="language">en-us</property>
+                <property name="preview-text"/>
+                <signal name="font-set" handler="text_font_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
                 <property name="top-attach">6</property>
               </packing>
             </child>
             <child>
               <object class="GtkLabel">
-                <property name="name">text_background_colour_label</property>
+                <property name="name">text_font_label</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
-                <property name="label" translatable="yes">Background Colour</property>
+                <property name="label" translatable="yes">Font</property>
                 <property name="xalign">0</property>
               </object>
               <packing>
                 <property name="left-attach">0</property>
-                <property name="top-attach">7</property>
+                <property name="top-attach">6</property>
               </packing>
             </child>
             <child>
               <object class="GtkLabel">
-                <property name="name">text_colour_label</property>
+                <property name="name">text_channel_label</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
-                <property name="label" translatable="yes">Text Colour</property>
+                <property name="label" translatable="yes">Channel</property>
                 <property name="xalign">0</property>
               </object>
               <packing>
                 <property name="left-attach">0</property>
-                <property name="top-attach">6</property>
+                <property name="top-attach">5</property>
               </packing>
             </child>
             <child>
-              <object class="GtkFontButton">
-                <property name="name">text_font</property>
+              <object class="GtkComboBoxText">
+                <property name="name">text_channel</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
+                <property name="top-attach">5</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkButton">
+                <property name="label" translatable="yes">Refresh List</property>
+                <property name="name">text_refresh_server_button</property>
                 <property name="visible">True</property>
                 <property name="can-focus">True</property>
                 <property name="receives-default">True</property>
-                <property name="font">Sans 12</property>
-                <property name="language">en-us</property>
-                <property name="preview-text"/>
-                <signal name="font-set" handler="text_font_changed" swapped="no"/>
+                <signal name="pressed" handler="text_server_refresh" swapped="no"/>
               </object>
               <packing>
                 <property name="left-attach">1</property>
-                <property name="top-attach">5</property>
+                <property name="top-attach">4</property>
               </packing>
             </child>
             <child>
               <object class="GtkLabel">
-                <property name="name">text_font_label</property>
+                <property name="name">text_server_label</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
-                <property name="label" translatable="yes">Font</property>
+                <property name="label" translatable="yes">Server</property>
                 <property name="xalign">0</property>
               </object>
               <packing>
                 <property name="left-attach">0</property>
-                <property name="top-attach">5</property>
+                <property name="top-attach">3</property>
               </packing>
             </child>
             <child>
               <object class="GtkComboBoxText">
-                <property name="name">text_channel</property>
+                <property name="name">text_server</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
               </object>
               <packing>
                 <property name="left-attach">1</property>
-                <property name="top-attach">4</property>
+                <property name="top-attach">3</property>
               </packing>
             </child>
             <child>
               <object class="GtkLabel">
-                <property name="name">text_channel_label</property>
+                <property name="name">text_popup_time_label</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
-                <property name="label" translatable="yes">Channel</property>
+                <property name="label" translatable="yes">Popup time limit</property>
                 <property name="xalign">0</property>
               </object>
               <packing>
                 <property name="left-attach">0</property>
-                <property name="top-attach">4</property>
+                <property name="top-attach">2</property>
               </packing>
             </child>
             <child>
-              <object class="GtkButton">
-                <property name="label" translatable="yes">Refresh List</property>
-                <property name="name">text_refresh_server_button</property>
+              <object class="GtkSpinButton">
+                <property name="name">text_popup_time</property>
                 <property name="visible">True</property>
                 <property name="can-focus">True</property>
-                <property name="receives-default">True</property>
-                <signal name="pressed" handler="text_server_refresh" swapped="no"/>
+                <property name="adjustment">text_popup_time_adj</property>
+                <signal name="value-changed" handler="text_popup_time_changed" swapped="no"/>
               </object>
               <packing>
                 <property name="left-attach">1</property>
-                <property name="top-attach">3</property>
+                <property name="top-attach">2</property>
               </packing>
             </child>
             <child>
               <placeholder/>
             </child>
+            <child>
+              <placeholder/>
+            </child>
           </object>
           <packing>
             <property name="position">2</property>
           </packing>
         </child>
         <child type="tab">
           <object class="GtkLabel" id="notebook_text_label">
```

### Comparing `discover-overlay-0.6.3/discover_overlay/image_getter.py` & `discover-overlay-0.6.5/discover_overlay/image_getter.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover_overlay/locales/cy/LC_MESSAGES/default.mo` & `discover-overlay-0.6.5/discover_overlay/locales/cy/LC_MESSAGES/default.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -82,23 +82,17 @@
 "sgrin. Rydym yn llwyr gefnogi amgylcheddau X11 a wlroots. Roeddem yn "
 "teimlo'r angen i wneud y prosiect hwn oherwydd y diffygion yn y gefnogaeth "
 "ar Linux gan y cleient anghytgord swyddogol."
 
 msgid "Display Horizontally"
 msgstr "Arddangos yn llorweddol"
 
-msgid "Display Icon Only"
-msgstr "Dangos eicon yn unig"
-
 msgid "Display Speakers Only"
 msgstr "Dangos siaradwyr yn unig"
 
-msgid "Dummy Count"
-msgstr "Nifer y dymis"
-
 msgid "Enable"
 msgstr "Galluogi"
 
 msgid "Fancy Avatar Shapes"
 msgstr "Siâp avatar ffansi"
 
 msgid "Floating"
@@ -136,17 +130,14 @@
 
 msgid "Icon Position"
 msgstr "Swydd Eicon"
 
 msgid "Icon Size"
 msgstr "Maint eicon"
 
-msgid "Icon Spacing"
-msgstr "Bylchiad eiconau"
-
 msgid "Idle"
 msgstr "Segur"
 
 msgid "Last Spoken"
 msgstr "Siaradwyd ddiwethaf"
 
 msgid "Left"
@@ -175,17 +166,14 @@
 
 msgid "Notification"
 msgstr "Hysbysiad"
 
 msgid "Open configuration window"
 msgstr "gan y cleient Discord"
 
-msgid "Order Avatars By"
-msgstr "Archebu avatars yn ôl"
-
 msgid "Overflow Style"
 msgstr "Arddull gorlifo"
 
 msgid "Overlay Location"
 msgstr "Lleoliad troslun"
 
 msgid "Overview"
```

### Comparing `discover-overlay-0.6.3/discover_overlay/notification_overlay.py` & `discover-overlay-0.6.5/discover_overlay/notification_overlay.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover_overlay/overlay.py` & `discover-overlay-0.6.5/discover_overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.6.3/discover_overlay/settings_window.py` & `discover-overlay-0.6.5/discover_overlay/settings_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -306,14 +306,17 @@
 
         self.widget['voice_highlight_self'].set_active(
             config.getboolean("main", "highlight_self", fallback=False))
 
         self.widget['voice_display_speakers_only'].set_active(
             config.getboolean("main", "only_speaking", fallback=False))
 
+        self.widget['voice_display_speakers_grace_period'].set_value(
+            config.getint("main", "only_speaking_grace", fallback=0))
+
         self.widget['voice_show_test_content'].set_active(
             config.getboolean("main", "show_dummy", fallback=False))
 
         self.widget['voice_talking_foreground'].set_rgba(self.make_colour(config.get(
             "main", "fg_hi_col", fallback="[1.0,1.0,1.0,1.0]")))
 
         self.widget['voice_talking_background'].set_rgba(self.make_colour(config.get(
@@ -345,16 +348,17 @@
 
         self.widget['voice_nick_length'].set_value(
             config.getint("main", "nick_length", fallback=32))
 
         self.widget['voice_avatar_size'].set_value(
             config.getint("main", "avatar_size", fallback=48))
 
-        self.widget['voice_display_icon_only'].set_active(config.getboolean(
-            "main", "icon_only", fallback=False))
+        show_name = not config.getboolean("main", "icon_only", fallback=False)
+        self.widget['voice_display_icon_only'].set_active(show_name)
+        self.voice_show_name_hide_others(show_name)
 
         self.widget['voice_square_avatar'].set_active(config.getboolean(
             "main", "square_avatar", fallback=True))
 
         self.widget['voice_fancy_avatar_shapes'].set_active(config.getboolean("main",
                                                                               "fancy_border", fallback=True))
 
@@ -366,14 +370,19 @@
 
         self.widget['voice_overflow_style'].set_active(
             config.getint("main", "overflow", fallback=0))
 
         self.widget['voice_show_title'].set_active(config.getboolean(
             "main", "show_title", fallback=False))
 
+        show_avatar = config.getboolean(
+            "main", "show_avatar", fallback=True)
+        self.widget['voice_show_avatar'].set_active(show_avatar)
+        self.voice_show_avatar_hide_others(show_avatar)
+
         self.widget['voice_show_connection_status'].set_active(config.getboolean(
             "main", "show_connection", fallback=False))
 
         self.widget['voice_show_disconnected'].set_active(config.getboolean(
             "main", "show_disconnected", fallback=False))
 
         self.widget['voice_dummy_count'].set_value(
@@ -390,14 +399,18 @@
 
         self.widget['text_enable'].set_active(
             config.getboolean("text", "enabled", fallback=False))
 
         self.widget['text_popup_style'].set_active(
             config.getboolean("text", "popup_style", fallback=False))
 
+        self.widget['text_popup_time'].set_value(
+            config.getint("text","text_time", fallback=30)
+        )
+
         self.current_guild = config.get("text", "guild", fallback="0")
 
         self.current_channel = config.get("text", "channel", fallback="0")
 
         font = config.get("text", "font", fallback=None)
         if font:
             self.widget['text_font'].set_font(font)
@@ -637,14 +650,16 @@
             self.voice_floating_x = pos_x
             self.voice_floating_y = pos_y
             self.voice_floating_w = width
             self.voice_floating_h = height
 
             config = ConfigParser(interpolation=None)
             config.read(self.config_file)
+            if not "main" in config.sections():
+                config.add_section("main")
             config.set("main", "floating_x", "%s" %
                        (int(self.voice_floating_x)))
             config.set("main", "floating_y", "%s" %
                        (int(self.voice_floating_y)))
             config.set("main", "floating_w", "%s" %
                        (int(self.voice_floating_w)))
             config.set("main", "floating_h", "%s" %
@@ -682,14 +697,16 @@
             self.text_floating_x = pos_x
             self.text_floating_y = pos_y
             self.text_floating_w = width
             self.text_floating_h = height
 
             config = ConfigParser(interpolation=None)
             config.read(self.config_file)
+            if not "text" in config.sections():
+                config.add_section("text")
             config.set("text", "floating_x", "%s" %
                        (int(self.text_floating_x)))
             config.set("text", "floating_y", "%s" %
                        (int(self.text_floating_y)))
             config.set("text", "floating_w", "%s" %
                        (int(self.text_floating_w)))
             config.set("text", "floating_h", "%s" %
@@ -798,14 +815,17 @@
 
     def voice_highlight_self_changed(self, button):
         self.config_set("main", "highlight_self", "%s" % (button.get_active()))
 
     def voice_display_speakers_only(self, button):
         self.config_set("main", "only_speaking", "%s" % (button.get_active()))
 
+    def voice_display_speakers_grace_period(self, button):
+        self.config_set("main", "only_speaking_grace", "%s" % (int(button.get_value())))
+
     def voice_toggle_test_content(self, button):
         self.config_set("main", "show_dummy", "%s" % (button.get_active()))
 
     def voice_talking_foreground_changed(self, button):
         colour = button.get_rgba()
         colour = [colour.red, colour.green, colour.blue, colour.alpha]
         self.config_set("main", "fg_hi_col", json.dumps(colour))
@@ -859,15 +879,16 @@
                         (int(button.get_value())))
 
     def voice_nick_length_changed(self, button):
         self.config_set("main", "nick_length", "%s" %
                         (int(button.get_value())))
 
     def voice_display_icon_only_changed(self, button):
-        self.config_set("main", "icon_only", "%s" % (button.get_active()))
+        self.config_set("main", "icon_only", "%s" % (not button.get_active()))
+        self.voice_show_name_hide_others(button.get_active())
 
     def voice_square_avatar_changed(self, button):
         self.config_set("main", "square_avatar", "%s" % (button.get_active()))
 
     def voice_fancy_avatar_shapes_changed(self, button):
         self.config_set("main", "fancy_border", "%s" % (button.get_active()))
 
@@ -892,20 +913,55 @@
         self.config_set("main", "show_disconnected", "%s" %
                         (button.get_active()))
 
     def voice_dummy_count_changed(self, button):
         self.config_set("main", "dummy_count", "%s" %
                         (int(button.get_value())))
 
+    def voice_show_avatar_changed(self, button):
+        self.config_set("main", "show_avatar", "%s" % (button.get_active()))
+        self.voice_show_avatar_hide_others(button.get_active())
+
+    def voice_show_name_hide_others(self, val):
+        if val:
+            # Show name options
+            self.widget['voice_font'].set_sensitive(True)
+            self.widget['voice_text_padding'].set_sensitive(True)
+            self.widget['voice_text_vertical_offset'].set_sensitive(True)
+            self.widget['voice_nick_length'].set_sensitive(True)
+        else:
+            # Hide name options
+            self.widget['voice_font'].set_sensitive(False)
+            self.widget['voice_text_padding'].set_sensitive(False)
+            self.widget['voice_text_vertical_offset'].set_sensitive(False)
+            self.widget['voice_nick_length'].set_sensitive(False)
+
+    def voice_show_avatar_hide_others(self, val):
+        if val:
+            # Show avatar options
+            self.widget['voice_square_avatar'].set_sensitive(True)
+            self.widget['voice_fancy_avatar_shapes'].set_sensitive(True)
+            self.widget['voice_avatar_size'].set_sensitive(True)
+            self.widget['voice_avatar_opacity'].set_sensitive(True)
+        else:
+            # Hide avatar options
+            self.widget['voice_square_avatar'].set_sensitive(False)
+            self.widget['voice_fancy_avatar_shapes'].set_sensitive(False)
+            self.widget['voice_avatar_size'].set_sensitive(False)
+            self.widget['voice_avatar_opacity'].set_sensitive(False)
+
     def text_enable_changed(self, button):
         self.config_set("text", "enabled", "%s" % (button.get_active()))
 
     def text_popup_style_changed(self, button):
         self.config_set("text", "popup_style", "%s" % (button.get_active()))
 
+    def text_popup_time_changed(self, button):
+        self.config_set("text", "text_time", "%s" % (int(button.get_value())))
+
     def text_server_changed(self, button):
         if button.get_active() < 0:
             self.config_set("text", "guild", "0")
             return
         guild = self.guild_ids[button.get_active()]
         if guild and self.current_guild != guild:
             self.current_guild = guild
```

### Comparing `discover-overlay-0.6.3/discover_overlay/text_overlay.py` & `discover-overlay-0.6.5/discover_overlay/text_overlay.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import cairo
 import gi
 from .image_getter import get_surface, draw_img_to_rect, get_aspected_size
 from .overlay import OverlayWindow
 gi.require_version("Gtk", "3.0")
 gi.require_version('PangoCairo', '1.0')
 # pylint: disable=wrong-import-position,wrong-import-order
-from gi.repository import Pango, PangoCairo  # nopep8
+from gi.repository import Pango, PangoCairo, GLib  # nopep8
 
 log = logging.getLogger(__name__)
 
 
 class TextOverlayWindow(OverlayWindow):
     """Overlay window for text"""
 
@@ -50,14 +50,20 @@
         self.attachment = {}
 
         self.image_list = []
         self.img_finder = re.compile(r"`")
         self.warned_filetypes = []
         self.set_title("Discover Text")
         self.redraw()
+        GLib.timeout_add_seconds(1, self.set_need_redraw)
+
+    def set_need_redraw(self):
+        if self.popup_style:
+            self.needsredraw = True
+        return True
 
     def set_blank(self):
         self.content = []
         self.needsredraw = True
 
     def tick(self):
         if len(self.attachment) > self.line_limit:
```

### Comparing `discover-overlay-0.6.3/discover_overlay/voice_overlay.py` & `discover-overlay-0.6.5/discover_overlay/voice_overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 import gettext
 import logging
 import math
 import cairo
 import sys
 import locale
 import pkg_resources
+from time import perf_counter
 from .overlay import OverlayWindow
 from .image_getter import get_surface, draw_img_to_rect, draw_img_to_mask
 # pylint: disable=wrong-import-order
 import gi
 gi.require_version("Gtk", "3.0")
 gi.require_version('PangoCairo', '1.0')
 # pylint: disable=wrong-import-position,wrong-import-order
-from gi.repository import Pango, PangoCairo  # nopep8
+from gi.repository import Pango, PangoCairo, GLib  # nopep8
 
 log = logging.getLogger(__name__)
 
 t = gettext.translation(
     'default', pkg_resources.resource_filename('discover_overlay', 'locales'), fallback=True)
 _ = t.gettext
 
@@ -40,14 +41,17 @@
 
     def __init__(self, discover, piggyback=None):
         OverlayWindow.__init__(self, discover, piggyback)
 
         self.avatars = {}
         self.avatar_masks = {}
 
+        # Cache for when somebody last spoke, used for "only_speaking" grace period
+        self.speaker_cache = {}
+
         self.dummy_data = []
         mostly_false = [False, False, False, False, False, False, False, True]
         for i in range(0, 100):
             speaking = mostly_false[random.randint(0, 7)]
             scream = ''
             if random.randint(0, 20) == 2:
                 scream = random.randint(8, 15)*'a'
@@ -59,14 +63,15 @@
                 "mute": False,
                 "deaf": mostly_false[random.randint(0, 7)],
                 "mute": mostly_false[random.randint(0, 7)],
                 "speaking": speaking,
                 'lastspoken': random.randint(2000, 2100) if speaking else random.randint(10, 30),
                 'friendlyname': name,
             })
+        self.show_avatar = True
         self.avatar_size = 48
         self.nick_length = 32
         self.text_pad = 6
         self.text_font = None
         self.title_font = None
         self.text_size = 13
         self.text_baseline_adj = 0
@@ -109,14 +114,20 @@
         self.guild_ids = tuple()
         self.force_location()
         get_surface(self.recv_avatar,
                     "share/icons/hicolor/256x256/apps/discover-overlay-default.png",
                     'def', self.avatar_size, self.icon_transparency)
         self.set_title("Discover Voice")
         self.redraw()
+        GLib.timeout_add_seconds(1, self.set_need_redraw)
+
+    def set_need_redraw(self):
+        if self.only_speaking:
+            self.needsredraw = True
+        return True
 
     def set_icon_transparency(self, trans):
         if self.icon_transparency == trans:
             return
         self.icon_transparency = trans
         get_surface(self.recv_avatar,
                     "share/icons/hicolor/256x256/apps/discover-overlay-default.png",
@@ -141,14 +152,18 @@
         self.title_font = font
         self.needsredraw = True
 
     def set_show_connection(self, show_connection):
         self.show_connection = show_connection
         self.needsredraw = True
 
+    def set_show_avatar(self, show_avatar):
+        self.show_avatar = show_avatar
+        self.needsredraw = True
+
     def set_show_title(self, show_title):
         self.show_title = show_title
         self.needsredraw = True
 
     def set_show_disconnected(self, show_disconnected):
         self.show_disconnected = show_disconnected
         self.needsredraw = True
@@ -299,14 +314,20 @@
 
     def set_only_speaking(self, only_speaking):
         """
         Set if overlay should only show people who are talking
         """
         self.only_speaking = only_speaking
 
+    def set_only_speaking_grace_period(self, grace_period):
+        """
+        Set grace period before hiding people who are not talking
+        """
+        self.only_speaking_grace_period = grace_period
+
     def set_highlight_self(self, highlight_self):
         """
         Set if the overlay should highlight the user
         """
         self.highlight_self = highlight_self
 
     def set_order(self, i):
@@ -464,41 +485,58 @@
 
             # Update friendly name with nick if possible
             if "nick" in user:
                 user["friendlyname"] = user["nick"]
             else:
                 user["friendlyname"] = user["username"]
 
-            # Remove users that arent speaking
+            # Remove users that haven't spoken within the grace period
             if self.only_speaking:
                 speaking = "speaking" in user and user["speaking"]
+
+                # Update the speaker cache
+                if speaking:
+                    self.speaker_cache[user["username"]] = perf_counter()
+
                 if not speaking:
-                    if user in users_to_draw:
+                    grace = self.only_speaking_grace_period
+
+                    if (
+                        grace > 0
+                        and (last_spoke := self.speaker_cache.get(user["username"]))
+                        and (perf_counter() - last_spoke) < grace
+                    ):
+                        # The user spoke within the grace period, so don't hide
+                        # them just yet
+                        pass
+
+                    elif user in users_to_draw:
                         users_to_draw.remove(user)
 
         if self.highlight_self:
             if self_user in users_to_draw:
                 users_to_draw.remove(self_user)
             users_to_draw.insert(0, self_user)
 
-        avatar_size = self.avatar_size
+        avatar_size = self.avatar_size if self.show_avatar else 0
+        line_height = self.avatar_size
         avatars_per_row = sys.maxsize
 
         # Calculate height needed to show overlay
         doTitle = False
         doConnection = False
         if self.show_connection:
             users_to_draw.insert(0, None)
             doConnection = True
         if self.show_title and self.channel_title:
             users_to_draw.insert(0, None)
             doTitle = True
 
         if self.horizontal:
-            needed_width = (len(users_to_draw) * self.avatar_size) + \
+            needed_width = (len(users_to_draw) * line_height) + \
                 (len(users_to_draw) + 1) * self.icon_spacing
 
             if needed_width > width:
                 if self.overflow == 1:  # Wrap
                     avatars_per_row = int(
                         width / (avatar_size+self.icon_spacing))
                 elif self.overflow == 2:  # Shrink
@@ -515,38 +553,38 @@
             rows_to_draw = []
             while len(users_to_draw) > 0:
                 row = []
                 for i in range(0, min(avatars_per_row, len(users_to_draw))):
                     row.append(users_to_draw.pop(0))
                 rows_to_draw.append(row)
             for row in rows_to_draw:
-                needed_width = (len(row) * (avatar_size + self.icon_spacing))
+                needed_width = (len(row) * (line_height + self.icon_spacing))
                 current_x = 0 + self.horz_edge_padding
                 if self.align_vert == 1:
                     current_x = (width / 2) - (needed_width) / 2
                 elif self.align_vert == 2:
                     current_x = width - needed_width - self.horz_edge_padding
 
                 for user in row:
                     if not user:
                         if doTitle:
                             doTitle = False
                             text_width = self.draw_title(
-                                context, current_x, current_y, avatar_size)
+                                context, current_x, current_y, avatar_size, line_height)
                         elif doConnection:
                             text_width = self.draw_connection(
-                                context, current_x, current_y, avatar_size)
+                                context, current_x, current_y, avatar_size, line_height)
                             doConnection = False
                     else:
                         self.draw_avatar(context, user, current_x,
-                                         current_y, avatar_size)
+                                         current_y, avatar_size, line_height)
                     current_x += avatar_size + self.icon_spacing
                 current_y += offset_y
         else:
-            needed_height = ((len(users_to_draw)+0) * self.avatar_size) + \
+            needed_height = ((len(users_to_draw)+0) * line_height) + \
                 (len(users_to_draw) + 1) * self.icon_spacing
 
             if needed_height > height:
                 if self.overflow == 1:  # Wrap
                     avatars_per_row = int(
                         height / (avatar_size + self.icon_spacing))
                 elif self.overflow == 2:  # Shrink
@@ -558,60 +596,61 @@
             current_x = 0 + self.horz_edge_padding
             offset_x_mult = 1
             offset_x = avatar_size + self.horz_edge_padding
             if self.align_right:
                 offset_x_mult = -1
                 current_x = self.width - avatar_size - self.horz_edge_padding
 
+
             # Choose where to start drawing
             current_y = 0 + self.vert_edge_padding
             if self.align_vert == 1:
                 current_y = (height / 2) - (needed_height / 2)
             elif self.align_vert == 2:
                 current_y = height - needed_height - self.vert_edge_padding
 
             cols_to_draw = []
             while len(users_to_draw) > 0:
                 col = []
                 for i in range(0, min(avatars_per_row, len(users_to_draw))):
                     col.append(users_to_draw.pop(0))
                 cols_to_draw.append(col)
             for col in cols_to_draw:
-                needed_height = (len(col) * (avatar_size + self.icon_spacing))
+                needed_height = (len(col) * (line_height + self.icon_spacing))
                 current_y = 0 + self.vert_edge_padding
                 if self.align_vert == 1:
                     current_y = (height/2) - (needed_height / 2)
                 elif self.align_vert == 2:
                     current_y = height - needed_height - self.vert_edge_padding
                 largest_text_width = 0
                 for user in col:
                     if not user:
                         if doTitle:
                             # Draw header
                             text_width = self.draw_title(
-                                context, current_x, current_y, avatar_size)
+                                context, current_x, current_y, avatar_size, line_height)
                             largest_text_width = max(
                                 text_width, largest_text_width)
-                            current_y += avatar_size + self.icon_spacing
+                            current_y += line_height + self.icon_spacing
                             doTitle = False
                         elif doConnection:
                             # Draw header
                             text_width = self.draw_connection(
-                                context, current_x, current_y, avatar_size)
+                                context, current_x, current_y, avatar_size, line_height)
                             largest_text_width = max(
                                 text_width, largest_text_width)
-                            current_y += avatar_size + self.icon_spacing
+                            current_y += line_height + self.icon_spacing
                             doConnection = False
 
                     else:
                         text_width = self.draw_avatar(
-                            context, user, current_x, current_y, avatar_size)
+                            context, user, current_x, current_y, avatar_size, line_height)
                         largest_text_width = max(
                             text_width, largest_text_width)
-                        current_y += avatar_size + self.icon_spacing
+                        current_y += line_height + self.icon_spacing
                 if largest_text_width > 0:
                     largest_text_width += self.text_pad
                 else:
                     largest_text_width = self.icon_spacing
                 current_x += offset_x_mult * (offset_x + largest_text_width)
 
         context.restore()
@@ -635,15 +674,15 @@
     def delete_avatar(self, identifier):
         """
         Remove avatar image
         """
         if identifier in self.avatars:
             del self.avatars[identifier]
 
-    def draw_title(self, context, pos_x, pos_y, avatar_size):
+    def draw_title(self, context, pos_x, pos_y, avatar_size, line_height):
         """
         Draw title at given Y position. Includes both text and image based on settings
         """
         tw = 0
         if not self.horizontal and not self.icon_only:
             title = self.channel_title
             if self.use_dummy:
@@ -651,14 +690,15 @@
             tw = self.draw_text(
                 context, title,
                 pos_x,
                 pos_y,
                 self.text_col,
                 self.norm_col,
                 avatar_size,
+                line_height,
                 self.title_font
             )
         if self.channel_icon:
             self.draw_avatar_pix(context, self.channel_icon, self.channel_mask,
                                  pos_x, pos_y, None, avatar_size)
         else:
             self.blank_avatar(context, pos_x, pos_y, avatar_size)
@@ -675,39 +715,40 @@
         _("AWAITING_ENDPOINT")
         _("AUTHENTICATING")
         _("CONNECTING")
         _("CONNECTED")
         _("VOICE_CONNECTING")
         _("VOICE_CONNECTED")
 
-    def draw_connection(self, context, pos_x, pos_y, avatar_size):
+    def draw_connection(self, context, pos_x, pos_y, avatar_size, line_height):
         """
         Draw title at given Y position. Includes both text and image based on settings
         """
         tw = 0
         if not self.horizontal and not self.icon_only:
             tw = self.draw_text(
                 context, _(self.connection_status),
                 pos_x,
                 pos_y,
                 self.text_col,
                 self.norm_col,
                 avatar_size,
+                line_height,
                 self.text_font
             )
         self.blank_avatar(context, pos_x, pos_y, avatar_size)
         self.draw_connection_icon(context, pos_x, pos_y, avatar_size)
         return tw
 
-    def draw_avatar(self, context, user, pos_x, pos_y, avatar_size):
+    def draw_avatar(self, context, user, pos_x, pos_y, avatar_size, line_height):
         """
         Draw avatar at given Y position. Includes both text and image based on settings
         """
         # Ensure pixbuf for avatar
-        if user["id"] not in self.avatars and user["avatar"]:
+        if user["id"] not in self.avatars and user["avatar"] and avatar_size>0:
             url = "https://cdn.discordapp.com/avatars/%s/%s.png" % (
                 user['id'], user['avatar'])
             get_surface(self.recv_avatar, url, user["id"],
                         self.avatar_size, self.icon_transparency)
 
             # Set the key with no value to avoid spamming requests
             self.avatars[user["id"]] = None
@@ -743,27 +784,28 @@
                 tw = self.draw_text(
                     context, user["friendlyname"],
                     pos_x,
                     pos_y,
                     fg_col,
                     bg_col,
                     avatar_size,
+                    line_height,
                     self.text_font
                 )
         self.draw_avatar_pix(context, pix, mask, pos_x,
                              pos_y, colour, avatar_size)
         if deaf:
             self.draw_deaf(context, pos_x, pos_y,
                            self.mute_bg_col, avatar_size)
         elif mute:
             self.draw_mute(context, pos_x, pos_y,
                            self.mute_bg_col, avatar_size)
         return tw
 
-    def draw_text(self, context, string, pos_x, pos_y, tx_col, bg_col, avatar_size, font):
+    def draw_text(self, context, string, pos_x, pos_y, tx_col, bg_col, avatar_size, line_height, font):
         """
         Draw username & background at given position
         """
         if self.nick_length < 32 and len(string) > self.nick_length:
             string = string[:(self.nick_length-1)] + u"\u2026"
 
         context.save()
@@ -777,15 +819,15 @@
             font = Pango.FontDescription(font)
             layout.set_font_description(font)
         (_ink_rect, logical_rect) = layout.get_pixel_extents()
         text_height = logical_rect.height
         text_width = logical_rect.width
 
         self.col(tx_col)
-        height_offset = (avatar_size / 2) - (text_height / 2)
+        height_offset = (line_height / 2) - (text_height / 2)
         text_y_offset = height_offset + self.text_baseline_adj
 
         if self.align_right:
             context.move_to(0, 0)
             self.col(bg_col)
             context.rectangle(
                 pos_x - text_width - (self.text_pad * 2),
@@ -833,15 +875,16 @@
         context.fill()
         context.restore()
 
     def draw_avatar_pix(self, context, pixbuf, mask, pos_x, pos_y, border_colour, avatar_size):
         """
         Draw avatar image at given position
         """
-
+        if not self.show_avatar:
+            return
         # Empty the space for this
         self.blank_avatar(context, pos_x, pos_y, avatar_size)
 
         # fallback default or fallback further to no image here
         if not pixbuf:
             pixbuf = self.def_avatar
             if not pixbuf:
@@ -906,14 +949,16 @@
                          avatar_size, avatar_size)
         context.restore()
 
     def draw_mute(self, context, pos_x, pos_y, bg_col, avatar_size):
         """
         Draw Mute logo
         """
+        if avatar_size <= 0:
+            return
         context.save()
         context.translate(pos_x, pos_y)
         context.scale(avatar_size, avatar_size)
 
         # Add a dark background
         context.set_operator(cairo.OPERATOR_ATOP)
         context.rectangle(0.0, 0.0, 1.0, 1.0)
@@ -973,14 +1018,16 @@
 
         context.restore()
 
     def draw_deaf(self, context, pos_x, pos_y, bg_col, avatar_size):
         """
         Draw deaf logo
         """
+        if avatar_size <= 0:
+            return
         context.save()
         context.translate(pos_x, pos_y)
         context.scale(avatar_size, avatar_size)
 
         # Add a dark background
         context.set_operator(cairo.OPERATOR_ATOP)
         context.rectangle(0.0, 0.0, 1.0, 1.0)
```

### Comparing `discover-overlay-0.6.3/discover_overlay.egg-info/PKG-INFO` & `discover-overlay-0.6.5/discover_overlay.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discover-overlay
-Version: 0.6.3
+Version: 0.6.5
 Summary: Voice chat overlay
 Home-page: https://github.com/trigg/Discover
 Author: trigg
 Author-email: 
 License: GPLv3+
 Keywords: discord overlay voice linux
 Classifier: Development Status :: 4 - Beta
@@ -85,19 +85,21 @@
 
 A compositor is strongly advised but there is a non-compositor mode optionally
 
 It is advised to install python-gobject from your system's own package manager.
 
 #### Debian/Ubuntu
 
-`apt install python3-gi python3-gi-cairo`
+`apt install python3-gi python3-gi-cairo libappindicator3-dev`
+
+Libappindicator might conflict with other installed packages, but is optional
 
 with Wayland support
 
-`apt install gtk-layer-shell`
+`apt install gtk-layer-shell libgtk-layer-shell-dev`
 
 #### Arch
 
 `pacman -S python-gobject libappindicator-gtk3`
 
 with Wayland support
```

### Comparing `discover-overlay-0.6.3/discover_overlay.egg-info/SOURCES.txt` & `discover-overlay-0.6.5/discover_overlay.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -25,10 +25,11 @@
 discover_overlay.egg-info/PKG-INFO
 discover_overlay.egg-info/SOURCES.txt
 discover_overlay.egg-info/dependency_links.txt
 discover_overlay.egg-info/entry_points.txt
 discover_overlay.egg-info/requires.txt
 discover_overlay.egg-info/top_level.txt
 discover_overlay/glade/settings.glade
-discover_overlay/glade/settings.glade~
 discover_overlay/locales/cy/LC_MESSAGES/default.mo
-discover_overlay/locales/en/LC_MESSAGES/default.mo
+discover_overlay/locales/de/LC_MESSAGES/default.mo
+discover_overlay/locales/en/LC_MESSAGES/default.mo
+discover_overlay/locales/tr/LC_MESSAGES/default.mo
```

### Comparing `discover-overlay-0.6.3/setup.py` & `discover-overlay-0.6.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     return open('README.md', 'r').read()
 
 
 setup(
     name='discover-overlay',
     author='trigg',
     author_email='',
-    version='0.6.3',
+    version='0.6.5',
     description='Voice chat overlay',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/trigg/Discover',
     packages=find_namespace_packages(),
     include_package_data=True,
     data_files=[
@@ -27,15 +27,16 @@
     ],
     install_requires=[
         'PyGObject>=3.22',
         'websocket-client',
         'pyxdg',
         'requests',
         'pillow',
-        'python-xlib'
+        'python-xlib',
+        'setuptools'
     ],
     entry_points={
         'console_scripts': [
             'discover-overlay = discover_overlay.discover_overlay:entrypoint',
         ]
     },
     classifiers=[
```


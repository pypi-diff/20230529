# Comparing `tmp/Photini-2023.5.1.tar.gz` & `tmp/Photini-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Photini-2023.5.1.tar", last modified: Mon May 22 14:35:21 2023, max compression
+gzip compressed data, was "/home/jim/Documents/projects/Photini/main/dist/tmpunar26eo/Photini-2023.5.2.tar", last modified: Mon May 29 10:47:18 2023, max compression
```

## Comparing `Photini-2023.5.1.tar` & `Photini-2023.5.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/
--rw-r--r--   0 jim       (1026) users      (100)    15878 2023-05-22 14:34:16.000000 Photini-2023.5.1/CHANGELOG.txt
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.5.1/LICENSE.txt
--rw-r--r--   0 jim       (1026) users      (100)      267 2023-05-17 06:57:34.000000 Photini-2023.5.1/MANIFEST.in
--rw-r--r--   0 jim       (1026) users      (100)     8969 2023-05-22 14:35:21.000000 Photini-2023.5.1/PKG-INFO
--rw-r--r--   0 jim       (1026) users      (100)     7859 2023-05-22 14:34:16.000000 Photini-2023.5.1/README.rst
--rw-r--r--   0 jim       (1026) users      (100)     2093 2023-05-17 06:57:34.000000 Photini-2023.5.1/pyproject.toml
--rw-r--r--   0 jim       (1026) users      (100)       38 2023-05-22 14:35:21.000000 Photini-2023.5.1/setup.cfg
--rw-r--r--   0 jim       (1026) users      (100)     4698 2023-05-17 06:57:34.000000 Photini-2023.5.1/setup.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/Photini.egg-info/
--rw-r--r--   0 jim       (1026) users      (100)     1707 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/Photini.egg-info/SOURCES.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/photini/
--rw-r--r--   0 jim       (1026) users      (100)      114 2023-05-22 14:34:16.000000 Photini-2023.5.1/src/photini/__init__.py
--rw-r--r--   0 jim       (1026) users      (100)      917 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/__main__.py
--rw-r--r--   0 jim       (1026) users      (100)    19936 2023-05-17 06:57:34.000000 Photini-2023.5.1/src/photini/address.py
--rw-r--r--   0 jim       (1026) users      (100)     4759 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/bingmap.py
--rw-r--r--   0 jim       (1026) users      (100)     5310 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/configstore.py
--rw-r--r--   0 jim       (1026) users      (100)     6890 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/cv.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/photini/data/
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/LICENSE.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/photini/data/bingmap/
--rw-r--r--   0 jim       (1026) users      (100)     7556 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/bingmap/script.js
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/photini/data/googlemap/
--rw-r--r--   0 jim       (1026) users      (100)     6239 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/googlemap/script.js
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/photini/data/icons/
--rw-r--r--   0 jim       (1026) users      (100)    14554 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/icons/photini_128.png
--rw-r--r--   0 jim       (1026) users      (100)     3262 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/icons/photini_48.png
--rw-r--r--   0 jim       (1026) users      (100)    86598 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/icons/photini_win.ico
--rw-r--r--   0 jim       (1026) users      (100)     2205 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/keys.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/photini/data/lang/
--rw-r--r--   0 jim       (1026) users      (100)    22137 2023-05-22 14:35:14.000000 Photini-2023.5.1/src/photini/data/lang/photini.ca.qm
--rw-r--r--   0 jim       (1026) users      (100)    32947 2023-05-22 14:35:13.000000 Photini-2023.5.1/src/photini/data/lang/photini.cs.qm
--rw-r--r--   0 jim       (1026) users      (100)    47740 2023-05-22 14:35:12.000000 Photini-2023.5.1/src/photini/data/lang/photini.de.qm
--rw-r--r--   0 jim       (1026) users      (100)    29131 2023-05-22 14:35:12.000000 Photini-2023.5.1/src/photini/data/lang/photini.en.qm
--rw-r--r--   0 jim       (1026) users      (100)    10685 2023-05-22 14:35:13.000000 Photini-2023.5.1/src/photini/data/lang/photini.es.qm
--rw-r--r--   0 jim       (1026) users      (100)    43018 2023-05-22 14:35:12.000000 Photini-2023.5.1/src/photini/data/lang/photini.fr.qm
--rw-r--r--   0 jim       (1026) users      (100)    55694 2023-05-22 14:35:13.000000 Photini-2023.5.1/src/photini/data/lang/photini.it.qm
--rw-r--r--   0 jim       (1026) users      (100)     2072 2023-05-22 14:35:14.000000 Photini-2023.5.1/src/photini/data/lang/photini.ko.qm
--rw-r--r--   0 jim       (1026) users      (100)    21280 2023-05-22 14:35:14.000000 Photini-2023.5.1/src/photini/data/lang/photini.nb.qm
--rw-r--r--   0 jim       (1026) users      (100)    10258 2023-05-22 14:35:14.000000 Photini-2023.5.1/src/photini/data/lang/photini.pl.qm
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/photini/data/linux/
--rw-r--r--   0 jim       (1026) users      (100)      991 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/linux/photini.desktop
--rw-r--r--   0 jim       (1026) users      (100)      209 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/map_circle_blue.png
--rw-r--r--   0 jim       (1026) users      (100)      207 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/map_circle_red.png
--rw-r--r--   0 jim       (1026) users      (100)     1867 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/map_pin_grey.png
--rw-r--r--   0 jim       (1026) users      (100)     2016 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/map_pin_red.png
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/photini/data/mapboxmap/
--rw-r--r--   0 jim       (1026) users      (100)     5715 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/mapboxmap/script.js
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-22 14:35:21.000000 Photini-2023.5.1/src/photini/data/windows/
--rw-r--r--   0 jim       (1026) users      (100)     2638 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/data/windows/install_shortcuts.vbs
--rw-r--r--   0 jim       (1026) users      (100)    13464 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/descriptive.py
--rw-r--r--   0 jim       (1026) users      (100)    23314 2023-05-22 14:34:16.000000 Photini-2023.5.1/src/photini/editor.py
--rw-r--r--   0 jim       (1026) users      (100)     8435 2023-05-17 06:57:34.000000 Photini-2023.5.1/src/photini/editsettings.py
--rw-r--r--   0 jim       (1026) users      (100)    32853 2023-05-22 14:34:16.000000 Photini-2023.5.1/src/photini/exiv2.py
--rw-r--r--   0 jim       (1026) users      (100)     3287 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/ffmpeg.py
--rw-r--r--   0 jim       (1026) users      (100)    33292 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/flickr.py
--rw-r--r--   0 jim       (1026) users      (100)     4191 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/googlemap.py
--rw-r--r--   0 jim       (1026) users      (100)    13099 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/googlephotos.py
--rw-r--r--   0 jim       (1026) users      (100)     4382 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/gpximporter.py
--rw-r--r--   0 jim       (1026) users      (100)    40241 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/imagelist.py
--rw-r--r--   0 jim       (1026) users      (100)    27611 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/importer.py
--rw-r--r--   0 jim       (1026) users      (100)    27252 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/ipernity.py
--rw-r--r--   0 jim       (1026) users      (100)     4396 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/loggerwindow.py
--rw-r--r--   0 jim       (1026) users      (100)     4235 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/mapboxmap.py
--rw-r--r--   0 jim       (1026) users      (100)    36681 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/metadata.py
--rw-r--r--   0 jim       (1026) users      (100)    21920 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/ownership.py
--rw-r--r--   0 jim       (1026) users      (100)    25788 2023-05-17 06:57:34.000000 Photini-2023.5.1/src/photini/photinimap.py
--rw-r--r--   0 jim       (1026) users      (100)    37738 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/pixelfed.py
--rw-r--r--   0 jim       (1026) users      (100)    10550 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/pyqt.py
--rw-r--r--   0 jim       (1026) users      (100)    36607 2023-05-22 14:34:16.000000 Photini-2023.5.1/src/photini/regions.py
--rw-r--r--   0 jim       (1026) users      (100)     6875 2023-05-17 06:57:34.000000 Photini-2023.5.1/src/photini/scripts.py
--rw-r--r--   0 jim       (1026) users      (100)     3687 2023-04-12 08:03:27.000000 Photini-2023.5.1/src/photini/spelling.py
--rw-r--r--   0 jim       (1026) users      (100)    40948 2023-05-22 14:34:16.000000 Photini-2023.5.1/src/photini/technical.py
--rw-r--r--   0 jim       (1026) users      (100)    72475 2023-05-22 14:34:16.000000 Photini-2023.5.1/src/photini/types.py
--rw-r--r--   0 jim       (1026) users      (100)    47789 2023-05-17 06:57:34.000000 Photini-2023.5.1/src/photini/uploader.py
--rw-r--r--   0 jim       (1026) users      (100)    35622 2023-05-22 14:34:16.000000 Photini-2023.5.1/src/photini/widgets.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:18.000000 Photini-2023.5.2/
+-rw-r--r--   0 jim       (1026) users      (100)    15957 2023-05-29 10:44:57.000000 Photini-2023.5.2/CHANGELOG.txt
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.5.2/LICENSE.txt
+-rw-r--r--   0 jim       (1026) users      (100)      267 2023-05-17 06:57:34.000000 Photini-2023.5.2/MANIFEST.in
+-rw-r--r--   0 jim       (1026) users      (100)     8969 2023-05-29 10:47:18.000000 Photini-2023.5.2/PKG-INFO
+-rw-r--r--   0 jim       (1026) users      (100)     7859 2023-05-22 14:34:16.000000 Photini-2023.5.2/README.rst
+-rw-r--r--   0 jim       (1026) users      (100)     2093 2023-05-17 06:57:34.000000 Photini-2023.5.2/pyproject.toml
+-rw-r--r--   0 jim       (1026) users      (100)       38 2023-05-29 10:47:18.000000 Photini-2023.5.2/setup.cfg
+-rw-r--r--   0 jim       (1026) users      (100)     4698 2023-05-17 06:57:34.000000 Photini-2023.5.2/setup.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:17.000000 Photini-2023.5.2/src/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:18.000000 Photini-2023.5.2/src/Photini.egg-info/
+-rw-r--r--   0 jim       (1026) users      (100)     1707 2023-05-29 10:47:17.000000 Photini-2023.5.2/src/Photini.egg-info/SOURCES.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:17.000000 Photini-2023.5.2/src/photini/
+-rw-r--r--   0 jim       (1026) users      (100)      114 2023-05-29 10:44:57.000000 Photini-2023.5.2/src/photini/__init__.py
+-rw-r--r--   0 jim       (1026) users      (100)      917 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/__main__.py
+-rw-r--r--   0 jim       (1026) users      (100)    19936 2023-05-17 06:57:34.000000 Photini-2023.5.2/src/photini/address.py
+-rw-r--r--   0 jim       (1026) users      (100)     4759 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/bingmap.py
+-rw-r--r--   0 jim       (1026) users      (100)     5310 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/configstore.py
+-rw-r--r--   0 jim       (1026) users      (100)     6890 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/cv.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:18.000000 Photini-2023.5.2/src/photini/data/
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/LICENSE.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:18.000000 Photini-2023.5.2/src/photini/data/bingmap/
+-rw-r--r--   0 jim       (1026) users      (100)     7556 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/bingmap/script.js
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:18.000000 Photini-2023.5.2/src/photini/data/googlemap/
+-rw-r--r--   0 jim       (1026) users      (100)     6239 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/googlemap/script.js
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:18.000000 Photini-2023.5.2/src/photini/data/icons/
+-rw-r--r--   0 jim       (1026) users      (100)    14554 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/icons/photini_128.png
+-rw-r--r--   0 jim       (1026) users      (100)     3262 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/icons/photini_48.png
+-rw-r--r--   0 jim       (1026) users      (100)    86598 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/icons/photini_win.ico
+-rw-r--r--   0 jim       (1026) users      (100)     2205 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/keys.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:18.000000 Photini-2023.5.2/src/photini/data/lang/
+-rw-r--r--   0 jim       (1026) users      (100)    22137 2023-05-29 10:45:32.000000 Photini-2023.5.2/src/photini/data/lang/photini.ca.qm
+-rw-r--r--   0 jim       (1026) users      (100)    32947 2023-05-29 10:45:31.000000 Photini-2023.5.2/src/photini/data/lang/photini.cs.qm
+-rw-r--r--   0 jim       (1026) users      (100)    47740 2023-05-29 10:45:30.000000 Photini-2023.5.2/src/photini/data/lang/photini.de.qm
+-rw-r--r--   0 jim       (1026) users      (100)    29131 2023-05-29 10:45:30.000000 Photini-2023.5.2/src/photini/data/lang/photini.en.qm
+-rw-r--r--   0 jim       (1026) users      (100)    10685 2023-05-29 10:45:30.000000 Photini-2023.5.2/src/photini/data/lang/photini.es.qm
+-rw-r--r--   0 jim       (1026) users      (100)    43018 2023-05-29 10:45:30.000000 Photini-2023.5.2/src/photini/data/lang/photini.fr.qm
+-rw-r--r--   0 jim       (1026) users      (100)    55694 2023-05-29 10:45:31.000000 Photini-2023.5.2/src/photini/data/lang/photini.it.qm
+-rw-r--r--   0 jim       (1026) users      (100)     2072 2023-05-29 10:45:31.000000 Photini-2023.5.2/src/photini/data/lang/photini.ko.qm
+-rw-r--r--   0 jim       (1026) users      (100)    21280 2023-05-29 10:45:32.000000 Photini-2023.5.2/src/photini/data/lang/photini.nb.qm
+-rw-r--r--   0 jim       (1026) users      (100)    10258 2023-05-29 10:45:31.000000 Photini-2023.5.2/src/photini/data/lang/photini.pl.qm
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:18.000000 Photini-2023.5.2/src/photini/data/linux/
+-rw-r--r--   0 jim       (1026) users      (100)      991 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/linux/photini.desktop
+-rw-r--r--   0 jim       (1026) users      (100)      209 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/map_circle_blue.png
+-rw-r--r--   0 jim       (1026) users      (100)      207 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/map_circle_red.png
+-rw-r--r--   0 jim       (1026) users      (100)     1867 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/map_pin_grey.png
+-rw-r--r--   0 jim       (1026) users      (100)     2016 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/map_pin_red.png
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:18.000000 Photini-2023.5.2/src/photini/data/mapboxmap/
+-rw-r--r--   0 jim       (1026) users      (100)     5715 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/mapboxmap/script.js
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-29 10:47:18.000000 Photini-2023.5.2/src/photini/data/windows/
+-rw-r--r--   0 jim       (1026) users      (100)     2638 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/data/windows/install_shortcuts.vbs
+-rw-r--r--   0 jim       (1026) users      (100)    13464 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/descriptive.py
+-rw-r--r--   0 jim       (1026) users      (100)    23314 2023-05-22 14:34:16.000000 Photini-2023.5.2/src/photini/editor.py
+-rw-r--r--   0 jim       (1026) users      (100)     8435 2023-05-17 06:57:34.000000 Photini-2023.5.2/src/photini/editsettings.py
+-rw-r--r--   0 jim       (1026) users      (100)    32853 2023-05-22 14:34:16.000000 Photini-2023.5.2/src/photini/exiv2.py
+-rw-r--r--   0 jim       (1026) users      (100)     3287 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/ffmpeg.py
+-rw-r--r--   0 jim       (1026) users      (100)    33292 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/flickr.py
+-rw-r--r--   0 jim       (1026) users      (100)     4191 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/googlemap.py
+-rw-r--r--   0 jim       (1026) users      (100)    13099 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/googlephotos.py
+-rw-r--r--   0 jim       (1026) users      (100)     4382 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/gpximporter.py
+-rw-r--r--   0 jim       (1026) users      (100)    40126 2023-05-29 10:44:57.000000 Photini-2023.5.2/src/photini/imagelist.py
+-rw-r--r--   0 jim       (1026) users      (100)    27611 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/importer.py
+-rw-r--r--   0 jim       (1026) users      (100)    27252 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/ipernity.py
+-rw-r--r--   0 jim       (1026) users      (100)     4396 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/loggerwindow.py
+-rw-r--r--   0 jim       (1026) users      (100)     4235 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/mapboxmap.py
+-rw-r--r--   0 jim       (1026) users      (100)    36703 2023-05-29 10:44:57.000000 Photini-2023.5.2/src/photini/metadata.py
+-rw-r--r--   0 jim       (1026) users      (100)    21920 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/ownership.py
+-rw-r--r--   0 jim       (1026) users      (100)    25788 2023-05-17 06:57:34.000000 Photini-2023.5.2/src/photini/photinimap.py
+-rw-r--r--   0 jim       (1026) users      (100)    37738 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/pixelfed.py
+-rw-r--r--   0 jim       (1026) users      (100)    10550 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/pyqt.py
+-rw-r--r--   0 jim       (1026) users      (100)    36607 2023-05-22 14:34:16.000000 Photini-2023.5.2/src/photini/regions.py
+-rw-r--r--   0 jim       (1026) users      (100)     6875 2023-05-17 06:57:34.000000 Photini-2023.5.2/src/photini/scripts.py
+-rw-r--r--   0 jim       (1026) users      (100)     3687 2023-04-12 08:03:27.000000 Photini-2023.5.2/src/photini/spelling.py
+-rw-r--r--   0 jim       (1026) users      (100)    40948 2023-05-22 14:34:16.000000 Photini-2023.5.2/src/photini/technical.py
+-rw-r--r--   0 jim       (1026) users      (100)    72475 2023-05-22 14:34:16.000000 Photini-2023.5.2/src/photini/types.py
+-rw-r--r--   0 jim       (1026) users      (100)    47789 2023-05-17 06:57:34.000000 Photini-2023.5.2/src/photini/uploader.py
+-rw-r--r--   0 jim       (1026) users      (100)    35622 2023-05-22 14:34:16.000000 Photini-2023.5.2/src/photini/widgets.py
```

### Comparing `Photini-2023.5.1/CHANGELOG.txt` & `Photini-2023.5.2/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see
 <http://www.gnu.org/licenses/>.
 
+Changes in v2023.5.2:
+  1/ Fix crash with PySide6 v6.5.1 when opening a file.
+
 Changes in v2023.5.1:
   1/ Tab labels use two lines instead of eliding to fit width.
   2/ Ignore NULL bytes in some phone images' Exif comment values.
   3/ Italian localisation is complete.
   4/ Other minor improvements and bug fixes.
 
 Changes in v2023.5.0:
```

### Comparing `Photini-2023.5.1/LICENSE.txt` & `Photini-2023.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/PKG-INFO` & `Photini-2023.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Photini
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Simple photo metadata editor
 Home-page: https://github.com/jim-easterbrook/Photini
 Author: Jim Easterbrook
 Author-email: jim@jim-easterbrook.me.uk
 License: GPLv3+
-Download-URL: https://github.com/jim-easterbrook/Photini/archive/2023.5.1.tar.gz
+Download-URL: https://github.com/jim-easterbrook/Photini/archive/2023.5.2.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `Photini-2023.5.1/README.rst` & `Photini-2023.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/pyproject.toml` & `Photini-2023.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/setup.py` & `Photini-2023.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/Photini.egg-info/SOURCES.txt` & `Photini-2023.5.2/src/Photini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/__main__.py` & `Photini-2023.5.2/src/photini/__main__.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/address.py` & `Photini-2023.5.2/src/photini/address.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/bingmap.py` & `Photini-2023.5.2/src/photini/bingmap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/configstore.py` & `Photini-2023.5.2/src/photini/configstore.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/cv.py` & `Photini-2023.5.2/src/photini/cv.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/LICENSE.txt` & `Photini-2023.5.2/src/photini/data/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/bingmap/script.js` & `Photini-2023.5.2/src/photini/data/bingmap/script.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/googlemap/script.js` & `Photini-2023.5.2/src/photini/data/googlemap/script.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/icons/photini_128.png` & `Photini-2023.5.2/src/photini/data/icons/photini_128.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/icons/photini_48.png` & `Photini-2023.5.2/src/photini/data/icons/photini_48.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/icons/photini_win.ico` & `Photini-2023.5.2/src/photini/data/icons/photini_win.ico`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/keys.txt` & `Photini-2023.5.2/src/photini/data/keys.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/lang/photini.ca.qm` & `Photini-2023.5.2/src/photini/data/lang/photini.ca.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/lang/photini.cs.qm` & `Photini-2023.5.2/src/photini/data/lang/photini.cs.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/lang/photini.de.qm` & `Photini-2023.5.2/src/photini/data/lang/photini.de.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/lang/photini.en.qm` & `Photini-2023.5.2/src/photini/data/lang/photini.en.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/lang/photini.es.qm` & `Photini-2023.5.2/src/photini/data/lang/photini.es.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/lang/photini.fr.qm` & `Photini-2023.5.2/src/photini/data/lang/photini.fr.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/lang/photini.it.qm` & `Photini-2023.5.2/src/photini/data/lang/photini.it.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/lang/photini.ko.qm` & `Photini-2023.5.2/src/photini/data/lang/photini.ko.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/lang/photini.nb.qm` & `Photini-2023.5.2/src/photini/data/lang/photini.nb.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/lang/photini.pl.qm` & `Photini-2023.5.2/src/photini/data/lang/photini.pl.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/linux/photini.desktop` & `Photini-2023.5.2/src/photini/data/linux/photini.desktop`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/map_pin_grey.png` & `Photini-2023.5.2/src/photini/data/map_pin_grey.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/map_pin_red.png` & `Photini-2023.5.2/src/photini/data/map_pin_red.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/mapboxmap/script.js` & `Photini-2023.5.2/src/photini/data/mapboxmap/script.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/data/windows/install_shortcuts.vbs` & `Photini-2023.5.2/src/photini/data/windows/install_shortcuts.vbs`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/descriptive.py` & `Photini-2023.5.2/src/photini/descriptive.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/editor.py` & `Photini-2023.5.2/src/photini/editor.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/editsettings.py` & `Photini-2023.5.2/src/photini/editsettings.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/exiv2.py` & `Photini-2023.5.2/src/photini/exiv2.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/ffmpeg.py` & `Photini-2023.5.2/src/photini/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/flickr.py` & `Photini-2023.5.2/src/photini/flickr.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/googlemap.py` & `Photini-2023.5.2/src/photini/googlemap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/googlephotos.py` & `Photini-2023.5.2/src/photini/googlephotos.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/gpximporter.py` & `Photini-2023.5.2/src/photini/gpximporter.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/imagelist.py` & `Photini-2023.5.2/src/photini/imagelist.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,26 +336,26 @@
     def get_selected(self):
         return self.selected
 
 
 class ScrollArea(QtWidgets.QScrollArea):
     dropped_images = QtSignal(list)
 
-    def __init__(self, parent=None):
+    def __init__(self, image_list=None, parent=None):
         super(ScrollArea, self).__init__(parent)
+        self.image_list = image_list
         self.setWidgetResizable(True)
         self.setAcceptDrops(True)
         widget = QtWidgets.QWidget()
         self.thumbs = ThumbsLayout(scroll_area=self)
         widget.setLayout(self.thumbs)
         self.setWidget(widget)
         # adopt some layout methods & signals
         self.add_widget = self.thumbs.addWidget
         self.remove_widget = self.thumbs.removeWidget
-        self.multi_row_changed = self.thumbs.multi_row_changed
 
     @catch_all
     def ensureWidgetVisible(self, widget):
         left, top, right, bottom = self.thumbs.getContentsMargins()
         super(ScrollArea, self).ensureWidgetVisible(
             widget, max(left, right), max(top, bottom))
 
@@ -386,22 +386,26 @@
     def set_minimum_height(self, min_height):
         bar = self.horizontalScrollBar()
         if bar.isVisible():
             min_height += bar.height()
         margins = self.contentsMargins()
         self.setMinimumHeight(min_height + margins.top() + margins.bottom())
 
+    @QtSlot()
+    @catch_all
+    def multi_row_changed(self):
+        if self.image_list.last_selected:
+            self.ensureWidgetVisible(self.image_list.last_selected)
+
 
 class ThumbsLayout(QtWidgets.QLayout):
     """Multi-row fixed-width or single-row variable-width grid of
     thumbnail widgets, according to height.
 
     """
-    multi_row_changed = QtSignal()
-
     def __init__(self, scroll_area=None, **kw):
         super(ThumbsLayout, self).__init__(**kw)
         self.scroll_area = scroll_area
         self.item_list = []
         self.multi_row = None
         self.do_layout()
 
@@ -455,15 +459,15 @@
             row_height = item_h + height_hint
             self.scroll_area.set_minimum_height(row_height)
             view_width, view_height = self.scroll_area.usable_size()
             multi_row = view_height > row_height
             if multi_row != self.multi_row:
                 self.multi_row = multi_row
                 # make selected item visible after redrawing has finished
-                QtCore.QTimer.singleShot(0, self.multi_row_changed.emit)
+                QtCore.QTimer.singleShot(0, self.scroll_area.multi_row_changed)
             if multi_row:
                 columns = max((view_width - width_hint) // item_w, 1)
                 rows = (len(self.item_list) + columns - 1) // columns
             else:
                 columns = len(self.item_list)
                 rows = 1
             width_hint += columns * item_w
@@ -502,18 +506,16 @@
         self.thumb_size = self.app.config_store.get('controls', 'thumb_size', 4)
         if self.thumb_size > 20:
             # old config, in pixels
             self.thumb_size = self.thumb_size // 20
         # thumbnail display
         self.setLayout(QtWidgets.QVBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
-        self.scroll_area = ScrollArea()
+        self.scroll_area = ScrollArea(image_list=self)
         self.scroll_area.dropped_images.connect(self.open_file_list)
-        self.scroll_area.multi_row_changed.connect(
-            self._ensure_selected_visible)
         self.layout().addWidget(self.scroll_area)
         QtGui2.QShortcut(QtGui.QKeySequence.StandardKey.MoveToPreviousChar,
                          self.scroll_area, self.move_to_prev_thumb)
         QtGui2.QShortcut(QtGui.QKeySequence.StandardKey.MoveToNextChar,
                          self.scroll_area, self.move_to_next_thumb)
         QtGui2.QShortcut(QtGui.QKeySequence.StandardKey.MoveToStartOfLine,
                          self.scroll_area, self.move_to_first_thumb)
@@ -672,20 +674,14 @@
 
     @QtSlot()
     @catch_all
     def _new_sort_order(self):
         self._sort_thumbnails()
         self.sort_order_changed.emit()
 
-    @QtSlot()
-    @catch_all
-    def _ensure_selected_visible(self):
-        if self.last_selected:
-            self.scroll_area.ensureWidgetVisible(self.last_selected)
-
     def _sort_thumbnails(self):
         sort_date = self.sort_date.isChecked()
         self.app.config_store.set('controls', 'sort_date', sort_date)
         with Busy():
             if sort_date:
                 self.images.sort(key=self._date_key)
             else:
```

### Comparing `Photini-2023.5.1/src/photini/importer.py` & `Photini-2023.5.2/src/photini/importer.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/ipernity.py` & `Photini-2023.5.2/src/photini/ipernity.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/loggerwindow.py` & `Photini-2023.5.2/src/photini/loggerwindow.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/mapboxmap.py` & `Photini-2023.5.2/src/photini/mapboxmap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/metadata.py` & `Photini-2023.5.2/src/photini/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,17 +231,17 @@
             os.utime(self._path, file_times)
         # check that data really was saved
         OK = True
         saved_tags = self.open_old(self._path).get_all_tags()
         for tag in self.get_all_tags():
             if tag in saved_tags:
                 continue
-            if tag in ('Exif.Image.GPSTag', 'Exif.MakerNote.ByteOrder',
-                       'Exif.MakerNote.Offset', 'Exif.Photo.MakerNote',
-                       'Exif.Image.IPTCNAA'):
+            if tag in ('Exif.Image.ExifTag', 'Exif.Image.GPSTag',
+                       'Exif.MakerNote.ByteOrder', 'Exif.MakerNote.Offset',
+                       'Exif.Photo.MakerNote', 'Exif.Image.IPTCNAA'):
                 # some tags disappear with good reason
                 continue
             family, group, tagname = tag.split('.', 2)
             if family == 'Exif' and group[:5] in (
                     'Canon', 'Casio', 'Fujif', 'Minol', 'Nikon', 'Olymp',
                     'Panas', 'Penta', 'Samsu', 'Sigma', 'Sony1'):
                 # maker note tags are often not saved
```

### Comparing `Photini-2023.5.1/src/photini/ownership.py` & `Photini-2023.5.2/src/photini/ownership.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/photinimap.py` & `Photini-2023.5.2/src/photini/photinimap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/pixelfed.py` & `Photini-2023.5.2/src/photini/pixelfed.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/pyqt.py` & `Photini-2023.5.2/src/photini/pyqt.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/regions.py` & `Photini-2023.5.2/src/photini/regions.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/scripts.py` & `Photini-2023.5.2/src/photini/scripts.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/spelling.py` & `Photini-2023.5.2/src/photini/spelling.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/technical.py` & `Photini-2023.5.2/src/photini/technical.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/types.py` & `Photini-2023.5.2/src/photini/types.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/uploader.py` & `Photini-2023.5.2/src/photini/uploader.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.5.1/src/photini/widgets.py` & `Photini-2023.5.2/src/photini/widgets.py`

 * *Files identical despite different names*


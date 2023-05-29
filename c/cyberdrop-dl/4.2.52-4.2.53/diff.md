# Comparing `tmp/cyberdrop-dl-4.2.52.tar.gz` & `tmp/cyberdrop-dl-4.2.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.52.tar", last modified: Mon May 29 04:37:18 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.53.tar", last modified: Mon May 29 15:28:13 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.52.tar` & `cyberdrop-dl-4.2.53.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:18.338169 cyberdrop-dl-4.2.52/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-29 04:37:18.338169 cyberdrop-dl-4.2.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:18.330168 cyberdrop-dl-4.2.52/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:18.330168 cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:18.330168 cyberdrop-dl-4.2.52/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:18.334169 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:18.338169 cyberdrop-dl-4.2.52/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:18.338169 cyberdrop-dl-4.2.52/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:37:18.330168 cyberdrop-dl-4.2.52/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-29 04:37:18.000000 cyberdrop-dl-4.2.52/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-29 04:37:18.000000 cyberdrop-dl-4.2.52/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:37:18.000000 cyberdrop-dl-4.2.52/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 04:37:18.000000 cyberdrop-dl-4.2.52/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-29 04:37:18.000000 cyberdrop-dl-4.2.52/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 04:37:18.000000 cyberdrop-dl-4.2.52/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-29 04:37:18.338169 cyberdrop-dl-4.2.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 04:37:09.000000 cyberdrop-dl-4.2.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.454269 cyberdrop-dl-4.2.53/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-29 15:28:13.454269 cyberdrop-dl-4.2.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.446268 cyberdrop-dl-4.2.53/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.450269 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.450269 cyberdrop-dl-4.2.53/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.450269 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.454269 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.454269 cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:28:13.446268 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 15:28:13.000000 cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-29 15:28:13.454269 cyberdrop-dl-4.2.53/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:28:04.000000 cyberdrop-dl-4.2.53/setup.py
```

### Comparing `cyberdrop-dl-4.2.52/LICENSE` & `cyberdrop-dl-4.2.53/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/PKG-INFO` & `cyberdrop-dl-4.2.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.52
+Version: 4.2.53
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.52 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.53 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.52/README.md` & `cyberdrop-dl-4.2.53/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/base_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,16 @@
 
 
 async def check_direct(url: URL) -> bool:
     """Checks whether the given url is a direct link to a content item"""
     mapping_direct = [r'i.pixl.li', r'i..pixl.li', r'img-...cyberdrop...', r'f.cyberdrop...',
                       r'fs-...cyberdrop...', r'jpg.church/images/...', r'simp..jpg.church', r'jpg.fish/images/...',
                       r'simp..jpg.fish', r'jpg.fishing/images/...', r'simp..jpg.fishing', r's..putmega.com',
-                      r's..putme.ga', r'images..imgbox.com', r's..lovefap...', r'img.kiwi/images/']
+                      r's..putme.ga', r'images..imgbox.com', r's..lovefap...', r'img.kiwi/images/',
+                      r'thumbs.gfycat.com/', r'giant.gfycat.com/']
     return any(re.search(domain, str(url)) for domain in mapping_direct)
 
 
 async def get_filename_and_ext(filename: str, forum: bool = False) -> Tuple[str, str]:
     """Returns the filename and extension of a given file, throws NoExtensionFailure if there is no extension"""
     filename_parts = filename.rsplit('.', 1)
     if len(filename_parts) == 1:
```

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from yarl import URL
 
-from ..base_functions.base_functions import create_media_item, log, logger
+from ..base_functions.base_functions import create_media_item, log, logger, check_direct
 from ..base_functions.data_classes import AlbumItem
 
 if TYPE_CHECKING:
     from ..base_functions.base_functions import ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
@@ -21,14 +21,21 @@
         self.error_writer = error_writer
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Basic scraper for gfycat"""
         album_obj = AlbumItem("Gfycat", [])
         try:
             log(f"Starting: {url}", quiet=self.quiet, style="green")
+            if await check_direct(url):
+                media_item = await create_media_item(url, url, self.SQL_Helper, "gfycat")
+                await album_obj.add_media(media_item)
+                await self.SQL_Helper.insert_album("gfycat", url, album_obj)
+                log(f"Finished: {url}", quiet=self.quiet, style="green")
+                return album_obj
+
             soup = await session.get_BS4(url)
 
             video = soup.select_one("video[class='video media']")
             video_srcs = video.select("source")
 
             video_link = None
             for src in video_srcs:
```

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.53/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.52
+Version: 4.2.53
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.52 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.53 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.52/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.53/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.52/setup.cfg` & `cyberdrop-dl-4.2.53/setup.cfg`

 * *Files identical despite different names*


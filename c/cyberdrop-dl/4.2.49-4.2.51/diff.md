# Comparing `tmp/cyberdrop-dl-4.2.49.tar.gz` & `tmp/cyberdrop-dl-4.2.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.49.tar", last modified: Sun May 28 21:25:00 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.51.tar", last modified: Mon May 29 04:24:33 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.49.tar` & `cyberdrop-dl-4.2.51.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.694375 cyberdrop-dl-4.2.49/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.694375 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.694375 cyberdrop-dl-4.2.49/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:00.694375 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 21:25:00.000000 cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-28 21:25:00.698375 cyberdrop-dl-4.2.49/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:24:51.000000 cyberdrop-dl-4.2.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:33.732524 cyberdrop-dl-4.2.51/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-29 04:24:33.732524 cyberdrop-dl-4.2.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:33.724524 cyberdrop-dl-4.2.51/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:33.728524 cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:33.728524 cyberdrop-dl-4.2.51/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:33.732524 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:33.732524 cyberdrop-dl-4.2.51/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:33.732524 cyberdrop-dl-4.2.51/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:33.724524 cyberdrop-dl-4.2.51/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-29 04:24:33.000000 cyberdrop-dl-4.2.51/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-29 04:24:33.000000 cyberdrop-dl-4.2.51/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:24:33.000000 cyberdrop-dl-4.2.51/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 04:24:33.000000 cyberdrop-dl-4.2.51/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-29 04:24:33.000000 cyberdrop-dl-4.2.51/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 04:24:33.000000 cyberdrop-dl-4.2.51/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-29 04:24:33.736524 cyberdrop-dl-4.2.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 04:24:24.000000 cyberdrop-dl-4.2.51/setup.py
```

### Comparing `cyberdrop-dl-4.2.49/LICENSE` & `cyberdrop-dl-4.2.51/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/PKG-INFO` & `cyberdrop-dl-4.2.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.49
+Version: 4.2.51
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.49 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.51 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.49/README.md` & `cyberdrop-dl-4.2.51/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,18 +61,18 @@
     config_group = config_data["Runtime"]
     runtime_opts = parser.add_argument_group("Runtime options")
     runtime_opts.add_argument("--allow-insecure-connections", help="allows insecure connections from content hosts", action="store_true")
     runtime_opts.add_argument("--attempts", type=int, help="number of attempts to download each file (default: %(default)s)", default=config_group["attempts"])
     runtime_opts.add_argument("--block-sub-folders", help="block sub folders from being created", action="store_true")
     runtime_opts.add_argument("--disable-attempt-limit", help="disables the attempt limitation", action="store_true")
     runtime_opts.add_argument("--include-id", help="include the ID in the download folder name", action="store_true")
-    runtime_opts.add_argument("--max_concurrent-threads", type=int, default=config_group["max_concurrent_threads"], help="Number of threads to download simultaneously (default: %(default)s)")
-    runtime_opts.add_argument("--max_concurrent-domains", type=int, default=config_group["max_concurrent_domains"], help="Number of domains to download simultaneously (default: %(default)s)")
-    runtime_opts.add_argument("--max_concurrent-albums", type=int, default=config_group["max_concurrent_albums"], help="Number of albums to download simultaneously (default: %(default)s)")
-    runtime_opts.add_argument("--max_concurrent-downloads-per-domain", type=int, default=config_group["max_concurrent_downloads_per_domain"], help="Number of simultaneous downloads per domain (default: %(default)s)")
+    runtime_opts.add_argument("--max-concurrent-threads", type=int, default=config_group["max_concurrent_threads"], help="Number of threads to download simultaneously (default: %(default)s)")
+    runtime_opts.add_argument("--max-concurrent-domains", type=int, default=config_group["max_concurrent_domains"], help="Number of domains to download simultaneously (default: %(default)s)")
+    runtime_opts.add_argument("--max-concurrent-albums", type=int, default=config_group["max_concurrent_albums"], help="Number of albums to download simultaneously (default: %(default)s)")
+    runtime_opts.add_argument("--max-concurrent-downloads-per-domain", type=int, default=config_group["max_concurrent_downloads_per_domain"], help="Number of simultaneous downloads per domain (default: %(default)s)")
     runtime_opts.add_argument("--skip-download-mark-completed", help="sets the scraped files as downloaded without downloading", action="store_true")
     runtime_opts.add_argument("--output-errored-urls", help="sets the failed urls to be output to the errored urls file", action="store_true")
     runtime_opts.add_argument("--output-unsupported-urls", help="sets the unsupported urls to be output to the unsupported urls file", action="store_true")
     runtime_opts.add_argument("--proxy", help="HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port]", default=config_group["proxy"])
     runtime_opts.add_argument("--remove-bunkr-identifier", help="removes the bunkr added identifier from output filenames", action="store_true")
     runtime_opts.add_argument("--required-free-space", type=int, default=config_group["required_free_space"], help="required free space (in gigabytes) for the program to run (default: %(default)s)")
```

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.51/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.51/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.49
+Version: 4.2.51
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.49 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.51 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.49/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.51/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.49/setup.cfg` & `cyberdrop-dl-4.2.51/setup.cfg`

 * *Files identical despite different names*


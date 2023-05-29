# Comparing `tmp/xklb-1.28.9.tar.gz` & `tmp/xklb-1.29.1.tar.gz`

## Comparing `xklb-1.28.9.tar` & `xklb-1.29.1.tar`

### file list

```diff
@@ -1,56 +1,59 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.28.9/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.28.9/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.28.9/Windows.md
--rw-r--r--   0        0        0   416121 2020-02-02 00:00:00.000000 xklb-1.28.9/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.28.9/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.28.9/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.28.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.28.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.28.9/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.28.9/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/__init__.py
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/books.py
--rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/consts.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/data.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/dl_config.py
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/dl_extract.py
--rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/fs_extract.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/lb.py
--rw-r--r--   0        0        0    37322 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/playback.py
--rw-r--r--   0        0        0    31511 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/praw_extract.py
--rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/stats.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21954 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/tube_extract.py
--rw-r--r--   0        0        0    29149 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.28.9/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.28.9/LICENSE
--rw-r--r--   0        0        0    40704 2020-02-02 00:00:00.000000 xklb-1.28.9/README.md
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 xklb-1.28.9/pyproject.toml
--rw-r--r--   0        0        0    44218 2020-02-02 00:00:00.000000 xklb-1.28.9/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.1/.gitattributes
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 xklb-1.29.1/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.1/Windows.md
+-rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.1/pdm.lock
+-rw-r--r--   0        0        0    17058 2020-02-02 00:00:00.000000 xklb-1.29.1/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.1/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.1/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/__init__.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/books.py
+-rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/consts.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/dl_config.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/dl_extract.py
+-rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/hn_extract.py
+-rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/lb.py
+-rw-r--r--   0        0        0    38063 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/playback.py
+-rw-r--r--   0        0        0    32826 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/search.py
+-rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/stats.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    23483 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/tube_extract.py
+-rw-r--r--   0        0        0    34064 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.1/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.1/LICENSE
+-rw-r--r--   0        0        0    41442 2020-02-02 00:00:00.000000 xklb-1.29.1/README.md
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 xklb-1.29.1/pyproject.toml
+-rw-r--r--   0        0        0    45038 2020-02-02 00:00:00.000000 xklb-1.29.1/PKG-INFO
```

### Comparing `xklb-1.28.9/Windows.md` & `xklb-1.29.1/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/pdm.lock` & `xklb-1.29.1/pdm.lock`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,22 @@
     "pathspec>=0.9.0",
     "platformdirs>=2",
     "tomli>=1.1.0; python_version < \"3.11\"",
     "typing-extensions>=3.10.0.0; python_version < \"3.10\"",
 ]
 
 [[package]]
+name = "blis"
+version = "0.7.9"
+summary = "The Blis BLAS-like linear algebra library, as a self-contained C-extension."
+dependencies = [
+    "numpy>=1.15.0",
+]
+
+[[package]]
 name = "brotab"
 version = "1.4.2"
 summary = "Control your browser's tabs from the command line"
 dependencies = [
     "Flask==2.0.2",
     "psutil==5.8.0",
     "requests==2.24.0",
@@ -128,14 +136,20 @@
 version = "0.2.1"
 summary = "YouTube chromecast api"
 dependencies = [
     "requests",
 ]
 
 [[package]]
+name = "catalogue"
+version = "2.0.8"
+requires_python = ">=3.6"
+summary = "Super lightweight function registries for your library"
+
+[[package]]
 name = "catt"
 version = "0.12.11"
 requires_python = ">=3.7"
 summary = "Cast All The Things allows you to send videos from many, many online sources to your Chromecast."
 dependencies = [
     "click>=7.1.2",
     "ifaddr>=0.1.7",
@@ -200,16 +214,31 @@
 
 [[package]]
 name = "compressed-rtf"
 version = "1.0.6"
 summary = "Compressed Rich Text Format (RTF) compression and decompression package"
 
 [[package]]
+name = "confection"
+version = "0.0.4"
+requires_python = ">=3.6"
+summary = "The sweetest config system for Python"
+dependencies = [
+    "pydantic!=1.8,!=1.8.1,<1.11.0,>=1.7.4",
+    "srsly<3.0.0,>=2.4.0",
+]
+
+[[package]]
+name = "cymem"
+version = "2.0.7"
+summary = "Manage calls to calloc/free through Cython"
+
+[[package]]
 name = "cython"
-version = "0.29.34"
+version = "0.29.35"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "The Cython compiler for writing C extensions for the Python language."
 
 [[package]]
 name = "decorator"
 version = "5.1.1"
 requires_python = ">=3.5"
@@ -218,15 +247,15 @@
 [[package]]
 name = "docx2txt"
 version = "0.8"
 summary = "A pure python-based utility to extract text and images from docx files."
 
 [[package]]
 name = "dogpile-cache"
-version = "1.2.0"
+version = "1.2.1"
 requires_python = ">=3.6"
 summary = "A caching front-end based on the Dogpile lock."
 dependencies = [
     "decorator>=4.0.0",
     "stevedore>=3.0.0",
 ]
 
@@ -302,15 +331,15 @@
 name = "future"
 version = "0.18.3"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Clean single-source support for Python 3 and 2"
 
 [[package]]
 name = "gallery-dl"
-version = "1.25.4"
+version = "1.25.5"
 requires_python = ">=3.4"
 summary = "Command-line program to download image galleries and collections from several image hosting sites"
 dependencies = [
     "requests>=2.11.0",
 ]
 
 [[package]]
@@ -434,14 +463,20 @@
 requires_python = ">=3.7"
 summary = "A very fast and expressive template engine."
 dependencies = [
     "MarkupSafe>=2.0",
 ]
 
 [[package]]
+name = "langcodes"
+version = "3.3.0"
+requires_python = ">=3.6"
+summary = "Tools for labeling human languages with IETF language tags"
+
+[[package]]
 name = "lxml"
 version = "4.9.2"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, != 3.4.*"
 summary = "Powerful and Pythonic XML processing library combining libxml2/libxslt with the ElementTree API."
 
 [[package]]
 name = "markdown"
@@ -485,14 +520,20 @@
 [[package]]
 name = "multidict"
 version = "6.0.4"
 requires_python = ">=3.7"
 summary = "multidict implementation"
 
 [[package]]
+name = "murmurhash"
+version = "1.0.9"
+requires_python = ">=3.6"
+summary = "Cython bindings for MurmurHash"
+
+[[package]]
 name = "mutagen"
 version = "1.46.0"
 requires_python = ">=3.7"
 summary = "read and write audio tags for many formats"
 
 [[package]]
 name = "mypy-extensions"
@@ -516,15 +557,15 @@
 name = "olefile"
 version = "0.46"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Python package to parse, read and write Microsoft OLE2 files (Structured Storage or Compound Document, Microsoft Office)"
 
 [[package]]
 name = "orjson"
-version = "3.8.12"
+version = "3.8.14"
 requires_python = ">=3.7"
 summary = "Fast, correct Python JSON library supporting dataclasses, datetimes, and numpy"
 
 [[package]]
 name = "packaging"
 version = "23.1"
 requires_python = ">=3.7"
@@ -553,14 +594,24 @@
 [[package]]
 name = "pathspec"
 version = "0.11.1"
 requires_python = ">=3.7"
 summary = "Utility library for gitignore style pattern matching of file paths."
 
 [[package]]
+name = "pathy"
+version = "0.10.1"
+requires_python = ">= 3.6"
+summary = "pathlib.Path subclasses for local and cloud bucket storage"
+dependencies = [
+    "smart-open<7.0.0,>=5.2.1",
+    "typer<1.0.0,>=0.3.0",
+]
+
+[[package]]
 name = "pbr"
 version = "5.11.1"
 requires_python = ">=2.6"
 summary = "Python Build Reasonableness"
 
 [[package]]
 name = "pdfminer-six"
@@ -621,25 +672,35 @@
 requires_python = "~=3.6"
 summary = "Low-level communication layer for PRAW 4+."
 dependencies = [
     "requests<3.0,>=2.6.0",
 ]
 
 [[package]]
+name = "preshed"
+version = "3.0.8"
+requires_python = ">=3.6"
+summary = "Cython hash table that trusts the keys are pre-hashed"
+dependencies = [
+    "cymem<2.1.0,>=2.0.2",
+    "murmurhash<1.1.0,>=0.28.0",
+]
+
+[[package]]
 name = "prompt-toolkit"
 version = "3.0.38"
 requires_python = ">=3.7.0"
 summary = "Library for building powerful interactive command lines in Python"
 dependencies = [
     "wcwidth",
 ]
 
 [[package]]
 name = "protobuf"
-version = "4.23.1"
+version = "4.23.2"
 requires_python = ">=3.7"
 summary = ""
 
 [[package]]
 name = "psutil"
 version = "5.8.0"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
@@ -669,25 +730,34 @@
 name = "pycparser"
 version = "2.21"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "C parser in Python"
 
 [[package]]
 name = "pycryptodome"
-version = "3.17"
+version = "3.18.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 summary = "Cryptographic library for Python"
 
 [[package]]
 name = "pycryptodomex"
-version = "3.17"
+version = "3.18.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 summary = "Cryptographic library for Python"
 
 [[package]]
+name = "pydantic"
+version = "1.10.8"
+requires_python = ">=3.7"
+summary = "Data validation and settings management using python type hints"
+dependencies = [
+    "typing-extensions>=4.2.0",
+]
+
+[[package]]
 name = "pyexiftool"
 version = "0.5.5"
 requires_python = ">=3.6"
 summary = "Python wrapper for exiftool"
 
 [[package]]
 name = "pygments"
@@ -811,15 +881,15 @@
     "markdown-it-py<3.0.0,>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.269"
+version = "0.0.270"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter, written in Rust."
 
 [[package]]
 name = "scalene"
 version = "1.5.19"
 requires_python = ">=3.8"
@@ -839,54 +909,120 @@
 summary = "Fetch location and size of physical screens."
 dependencies = [
     "Cython; sys_platform == \"darwin\"",
     "pyobjc-framework-Cocoa; sys_platform == \"darwin\"",
 ]
 
 [[package]]
+name = "setuptools"
+version = "67.8.0"
+requires_python = ">=3.7"
+summary = "Easily download, build, install, upgrade, and uninstall Python packages"
+
+[[package]]
 name = "six"
 version = "1.12.0"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*"
 summary = "Python 2 and 3 compatibility utilities"
 
 [[package]]
+name = "sklearn"
+version = "0.0.post5"
+summary = "deprecated sklearn package, use scikit-learn instead"
+
+[[package]]
+name = "smart-open"
+version = "6.3.0"
+requires_python = ">=3.6,<4.0"
+summary = "Utils for streaming large files (S3, HDFS, GCS, Azure Blob Storage, gzip, bz2...)"
+
+[[package]]
 name = "sortedcontainers"
 version = "2.4.0"
 summary = "Sorted Containers -- Sorted List, Sorted Dict, Sorted Set"
 
 [[package]]
 name = "soupsieve"
 version = "2.4.1"
 requires_python = ">=3.7"
 summary = "A modern CSS selector implementation for Beautiful Soup."
 
 [[package]]
+name = "spacy"
+version = "3.5.3"
+requires_python = ">=3.6"
+summary = "Industrial-strength Natural Language Processing (NLP) in Python"
+dependencies = [
+    "catalogue<2.1.0,>=2.0.6",
+    "cymem<2.1.0,>=2.0.2",
+    "jinja2",
+    "langcodes<4.0.0,>=3.2.0",
+    "murmurhash<1.1.0,>=0.28.0",
+    "numpy>=1.15.0",
+    "packaging>=20.0",
+    "pathy>=0.10.0",
+    "preshed<3.1.0,>=3.0.2",
+    "pydantic!=1.8,!=1.8.1,<1.11.0,>=1.7.4",
+    "requests<3.0.0,>=2.13.0",
+    "setuptools",
+    "smart-open<7.0.0,>=5.2.1",
+    "spacy-legacy<3.1.0,>=3.0.11",
+    "spacy-loggers<2.0.0,>=1.0.0",
+    "srsly<3.0.0,>=2.4.3",
+    "thinc<8.2.0,>=8.1.8",
+    "tqdm<5.0.0,>=4.38.0",
+    "typer<0.8.0,>=0.3.0",
+    "wasabi<1.2.0,>=0.9.1",
+]
+
+[[package]]
+name = "spacy-legacy"
+version = "3.0.12"
+requires_python = ">=3.6"
+summary = "Legacy registered functions for spaCy backwards compatibility"
+
+[[package]]
+name = "spacy-loggers"
+version = "1.0.4"
+requires_python = ">=3.6"
+summary = "Logging utilities for SpaCy"
+
+[[package]]
 name = "speechrecognition"
 version = "3.8.1"
 summary = "Library for performing speech recognition, with support for several engines and APIs, online and offline."
 
 [[package]]
 name = "sqlite-fts4"
 version = "1.0.3"
 summary = "Python functions for working with SQLite FTS4 search"
 
 [[package]]
 name = "sqlite-utils"
-version = "3.31"
+version = "3.32.1"
 requires_python = ">=3.7"
 summary = "CLI tool and Python library for manipulating SQLite databases"
 dependencies = [
     "click",
     "click-default-group-wheel",
     "python-dateutil",
     "sqlite-fts4",
     "tabulate",
 ]
 
 [[package]]
+name = "srsly"
+version = "2.4.6"
+requires_python = ">=3.6"
+summary = "Modern high-performance serialization utilities for Python"
+dependencies = [
+    "catalogue<2.1.0,>=2.0.3",
+]
+
+[[package]]
 name = "ssort"
 version = "0.11.6"
 requires_python = ">=3.8"
 summary = "The python statement sorter"
 dependencies = [
     "pathspec>=0.9.0",
 ]
@@ -951,34 +1087,72 @@
     "pdfminer-six==20191110",
     "python-pptx~=0.6.18",
     "six~=1.12.0",
     "xlrd~=1.2.0",
 ]
 
 [[package]]
+name = "thinc"
+version = "8.1.10"
+requires_python = ">=3.6"
+summary = "A refreshing functional take on deep learning, compatible with your favorite libraries"
+dependencies = [
+    "blis<0.8.0,>=0.7.8",
+    "catalogue<2.1.0,>=2.0.4",
+    "confection<1.0.0,>=0.0.1",
+    "cymem<2.1.0,>=2.0.2",
+    "murmurhash<1.1.0,>=1.0.2",
+    "numpy>=1.15.0",
+    "packaging>=20.0",
+    "preshed<3.1.0,>=3.0.2",
+    "pydantic!=1.8,!=1.8.1,<1.11.0,>=1.7.4",
+    "setuptools",
+    "srsly<3.0.0,>=2.4.0",
+    "wasabi<1.2.0,>=0.8.1",
+]
+
+[[package]]
 name = "tinytag"
 version = "1.9.0"
 requires_python = ">=2.7"
 summary = "Read music meta data and length of MP3, OGG, OPUS, MP4, M4A, FLAC, WMA and Wave files"
 
 [[package]]
 name = "tomli"
 version = "2.0.1"
 requires_python = ">=3.7"
 summary = "A lil' TOML parser"
 
 [[package]]
+name = "tqdm"
+version = "4.65.0"
+requires_python = ">=3.7"
+summary = "Fast, Extensible Progress Meter"
+dependencies = [
+    "colorama; platform_system == \"Windows\"",
+]
+
+[[package]]
 name = "traitlets"
 version = "5.9.0"
 requires_python = ">=3.7"
 summary = "Traitlets Python configuration system"
 
 [[package]]
+name = "typer"
+version = "0.7.0"
+requires_python = ">=3.6"
+summary = "Typer, build great CLIs. Easy to code. Based on Python type hints."
+dependencies = [
+    "click<9.0.0,>=7.1.1",
+]
+
+[[package]]
 name = "typing-extensions"
-version = "4.5.0"
+version = "4.6.2"
 requires_python = ">=3.7"
 summary = "Backported and Experimental Type Hints for Python 3.7+"
 
 [[package]]
 name = "tzdata"
 version = "2023.3"
 requires_python = ">=2"
@@ -1005,21 +1179,30 @@
 [[package]]
 name = "urllib3"
 version = "1.25.11"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, <4"
 summary = "HTTP library with thread-safe connection pooling, file post, and more."
 
 [[package]]
+name = "wasabi"
+version = "1.1.1"
+requires_python = ">=3.6"
+summary = "A lightweight console printing and formatting toolkit"
+dependencies = [
+    "colorama>=0.4.6; sys_platform == \"win32\" and python_version >= \"3.7\"",
+]
+
+[[package]]
 name = "wcwidth"
 version = "0.2.6"
 summary = "Measures the displayed width of unicode strings in a terminal"
 
 [[package]]
 name = "websocket-client"
-version = "1.5.1"
+version = "1.5.2"
 requires_python = ">=3.7"
 summary = "WebSocket client for Python with low level API options"
 
 [[package]]
 name = "websockets"
 version = "11.0.3"
 requires_python = ">=3.7"
@@ -1044,15 +1227,15 @@
 name = "xlrd"
 version = "1.2.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Library for developers to extract data from Microsoft Excel (tm) spreadsheet files"
 
 [[package]]
 name = "xlsxwriter"
-version = "3.1.0"
+version = "3.1.2"
 requires_python = ">=3.6"
 summary = "A Python module for creating Excel XLSX files."
 
 [[package]]
 name = "yarl"
 version = "1.9.2"
 requires_python = ">=3.7"
@@ -1074,15 +1257,15 @@
     "mutagen",
     "pycryptodomex",
     "websockets",
 ]
 
 [[package]]
 name = "zeroconf"
-version = "0.62.0"
+version = "0.63.0"
 requires_python = ">=3.7,<4.0"
 summary = "A pure python implementation of multicast DNS service discovery"
 dependencies = [
     "async-timeout>=3.0.0; python_version < \"3.11\"",
     "ifaddr>=0.1.7",
 ]
 
@@ -1092,15 +1275,15 @@
 requires_python = ">=3.7"
 summary = "Backport of pathlib-compatible object wrapper for zip files"
 
 [metadata]
 lock_version = "4.2"
 cross_platform = true
 groups = ["default", "all", "deluxe", "dev", "test"]
-content_hash = "sha256:707176187d52bfd11f71fd3d9998f736f44f8bfe637878e74e8948ec9f31c52c"
+content_hash = "sha256:838a39f6efcdf7890f45ea1f5c4bde5c496a26b207eb1344404bdaf9e0d230b0"
 
 [metadata.files]
 "aiohttp 3.8.4" = [
     {url = "https://files.pythonhosted.org/packages/03/e7/84b65e341b1f45753fea51158d8a9522e57a5ae804acbc6dc34edf07cea0/aiohttp-3.8.4-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:bca5f24726e2919de94f047739d0a4fc01372801a3672708260546aa2601bf57"},
     {url = "https://files.pythonhosted.org/packages/04/03/3ce412b191aba5961b4ada3ee7a93498623e218fb4d50ac6d357da61dc26/aiohttp-3.8.4-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:8189c56eb0ddbb95bfadb8f60ea1b22fcfa659396ea36f6adcc521213cd7b44d"},
     {url = "https://files.pythonhosted.org/packages/05/ee/77b3dc08f41a1bce842e30134233c58b3bbe8c0fa7be121295aa2fad885d/aiohttp-3.8.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:17b79c2963db82086229012cff93ea55196ed31f6493bb1ccd2c62f1724324e4"},
     {url = "https://files.pythonhosted.org/packages/07/3c/04c65b5873524a415509cbcf21787be32c31f4e729840fab9866dd197030/aiohttp-3.8.4-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:7c7837fe8037e96b6dd5cfcf47263c1620a9d332a87ec06a6ca4564e56bd0f36"},
@@ -1270,14 +1453,44 @@
     {url = "https://files.pythonhosted.org/packages/d6/36/66370f5017b100225ec4950a60caeef60201a10080da57ddb24124453fba/black-23.3.0.tar.gz", hash = "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940"},
     {url = "https://files.pythonhosted.org/packages/d7/6f/d3832960a3b646b333b7f0d80d336a3c123012e9d9d5dba4a622b2b6181d/black-23.3.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6"},
     {url = "https://files.pythonhosted.org/packages/db/f4/7908f71cc71da08df1317a3619f002cbf91927fb5d3ffc7723905a2113f7/black-23.3.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915"},
     {url = "https://files.pythonhosted.org/packages/de/b4/76f152c5eb0be5471c22cd18380d31d188930377a1a57969073b89d6615d/black-23.3.0-cp310-cp310-win_amd64.whl", hash = "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c"},
     {url = "https://files.pythonhosted.org/packages/eb/a5/17b40bfd9b607b69fa726b0b3a473d14b093dcd5191ea1a1dd664eccfee3/black-23.3.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b"},
     {url = "https://files.pythonhosted.org/packages/fd/5b/fc2d7922c1a6bb49458d424b5be71d251f2d0dc97be9534e35d171bdc653/black-23.3.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"},
 ]
+"blis 0.7.9" = [
+    {url = "https://files.pythonhosted.org/packages/07/0f/59e6458349338cbc968def7f215fa1ccb4ba03b913d4f0e55b4ab8e7c142/blis-0.7.9-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6d12475e588a322e66a18346a3faa9eb92523504042e665c193d1b9b0b3f0482"},
+    {url = "https://files.pythonhosted.org/packages/08/21/8a74aca8822867fd037bcf2b8948dc52fc68b19caf70e0aff067e094a02e/blis-0.7.9-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d4eb70a79562a211bd2e6b6db63f1e2eed32c0ab3e9ef921d86f657ae8375845"},
+    {url = "https://files.pythonhosted.org/packages/13/2f/ba6ea08896c308f2666fb3cc4ff29ab03aa062050cc11e76ee8a6ca6873b/blis-0.7.9-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b5f4691bf62013eccc167c38a85c09a0bf0c6e3e80d4c2229cdf2668c1124eb0"},
+    {url = "https://files.pythonhosted.org/packages/1a/9f/22d3e11da5103e7ecb2f49d2e9bd6ceee62070215a6cf9a9923c27ee7da1/blis-0.7.9-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f7b6315d7b1ac5546bc0350f5f8d7cc064438d23db19a5c21aaa6ae7d93c1ab5"},
+    {url = "https://files.pythonhosted.org/packages/28/b6/e1cdfcf4ada40bef7c0511576231df20ac94a15baeb7ceaab2a180463268/blis-0.7.9-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f5cec812ee47b29107eb36af9b457be7191163eab65d61775ed63538232c59d5"},
+    {url = "https://files.pythonhosted.org/packages/47/d3/a93226b247b8f423c946cf6f76675561fa166b5d5fd78b8671c95238cbff/blis-0.7.9-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d205a7e69523e2bacdd67ea906b82b84034067e0de83b33bd83eb96b9e844ae3"},
+    {url = "https://files.pythonhosted.org/packages/4c/20/abb520e063a8301527ba5b0c0e8c13b320ad61a948f94c557ed492776bbf/blis-0.7.9-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:179037cb5e6744c2e93b6b5facc6e4a0073776d514933c3db1e1f064a3253425"},
+    {url = "https://files.pythonhosted.org/packages/53/43/4b5d66ebc6631042361d7f9d88c1589f1e30a76e6bc11b7485df197a3109/blis-0.7.9-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:6fd5941bd5a21082b19d1dd0f6d62cd35609c25eb769aa3457d9877ef2ce37a9"},
+    {url = "https://files.pythonhosted.org/packages/59/32/f8c2b0385dcc3e70aed7f52116ce45e80d85f56dfba524f7d7d965e0c5df/blis-0.7.9-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c0521231bc95ab522f280da3bbb096299c910a62cac2376d48d4a1d403c54393"},
+    {url = "https://files.pythonhosted.org/packages/65/b9/5cd40f5981326c53cf5c00d7c88f2d6ff864105e82c740c2b0a58dc62224/blis-0.7.9-cp310-cp310-win_amd64.whl", hash = "sha256:d3882b4f44a33367812b5e287c0690027092830ffb1cce124b02f64e761819a4"},
+    {url = "https://files.pythonhosted.org/packages/6a/92/3a6b0718d2cec998a544365771d9db52d7ddd6d973c9db7e5c7ae82a493c/blis-0.7.9-cp36-cp36m-win_amd64.whl", hash = "sha256:d811e88480203d75e6e959f313fdbf3326393b4e2b317067d952347f5c56216e"},
+    {url = "https://files.pythonhosted.org/packages/6b/07/8c33738bb530e6b7bb4e869bf1ecb5901b30e413dfff0b80300d4ea0a523/blis-0.7.9-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c399a03de4059bf8e700b921f9ff5d72b2a86673616c40db40cd0592051bdd07"},
+    {url = "https://files.pythonhosted.org/packages/6f/36/103bd862bd8b8373cea47960273e4dfa89158a185934c00e3cbadbdfd66a/blis-0.7.9-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:d0e82a6e0337d5231129a4e8b36978fa7b973ad3bb0257fd8e3714a9b35ceffd"},
+    {url = "https://files.pythonhosted.org/packages/72/ce/3c36c93ce590aefd41c91332068bb2cd5f2d4e11a7dcd17f35ded050d497/blis-0.7.9-cp37-cp37m-win_amd64.whl", hash = "sha256:3e3f95e035c7456a1f5f3b5a3cfe708483a00335a3a8ad2211d57ba4d5f749a5"},
+    {url = "https://files.pythonhosted.org/packages/77/c8/330dd7d0d7f37198a6850fbad796ca94f15ab8d2e38d0b8d33bd46a6efe6/blis-0.7.9-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:db2959560dcb34e912dad0e0d091f19b05b61363bac15d78307c01334a4e5d9d"},
+    {url = "https://files.pythonhosted.org/packages/7c/36/eec5e1fd84c3078daa65823c6de8efbe5da3449dcfa763988c3afa232cbf/blis-0.7.9-cp38-cp38-win_amd64.whl", hash = "sha256:b8a1fcd2eb267301ab13e1e4209c165d172cdf9c0c9e08186a9e234bf91daa16"},
+    {url = "https://files.pythonhosted.org/packages/8c/fd/9f4502280a20262c6d63cd64be75f30c99116106b362fa6783ebb239910b/blis-0.7.9-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b9737035636452fb6d08e7ab79e5a9904be18a0736868a129179cd9f9ab59825"},
+    {url = "https://files.pythonhosted.org/packages/95/ac/0e8ecb3e862bec67f36ab26864ce6ef081b8f8c53e053cf23e8bcd31446c/blis-0.7.9-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:b3ea73707a7938304c08363a0b990600e579bfb52dece7c674eafac4bf2df9f7"},
+    {url = "https://files.pythonhosted.org/packages/99/90/188986a63b7c9df8689003a7b7c8d0490e07dc23216788c4ed29fbcbe511/blis-0.7.9-cp39-cp39-win_amd64.whl", hash = "sha256:d81c3f627d33545fc25c9dcb5fee66c476d89288a27d63ac16ea63453401ffd5"},
+    {url = "https://files.pythonhosted.org/packages/9d/7d/29bc4eebf798a727bf83cf944842828df1fb3a33b38c9eeb1f9aada96704/blis-0.7.9-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4d5755ef37a573647be62684ca1545698879d07321f1e5b89a4fd669ce355eb0"},
+    {url = "https://files.pythonhosted.org/packages/cb/61/22b8175ffebde4f5a6b1695d4186352af6850dfe4dc5024a7ca3624e71d2/blis-0.7.9-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:e85993364cae82707bfe7e637bee64ec96e232af31301e5c81a351778cb394b9"},
+    {url = "https://files.pythonhosted.org/packages/cd/97/0adeac2bb223b7e16854049e6f0d5d3526d7d79e4fe44f6454416531715e/blis-0.7.9-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:8275f6b6eee714b85f00bf882720f508ed6a60974bcde489715d37fd35529da8"},
+    {url = "https://files.pythonhosted.org/packages/cd/bb/4d3d7fbe08dda1a62fb3f89f8f2e04e5204d95c2c536183785938cf01818/blis-0.7.9-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:97ad55e9ef36e4ff06b35802d0cf7bfc56f9697c6bc9427f59c90956bb98377d"},
+    {url = "https://files.pythonhosted.org/packages/cf/51/cf0facfd2385a7c699f5a364cb7eba596f8c6e58c707ad0ea1e747710049/blis-0.7.9-cp311-cp311-win_amd64.whl", hash = "sha256:5fd46c649acd1920482b4f5556d1c88693cba9bf6a494a020b00f14b42e1132f"},
+    {url = "https://files.pythonhosted.org/packages/f1/06/779b16d3bdec58545e5ab7cfef12a179504720e73343d3c75571e700e33e/blis-0.7.9-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:5cb1db88ab629ccb39eac110b742b98e3511d48ce9caa82ca32609d9169a9c9c"},
+    {url = "https://files.pythonhosted.org/packages/f8/19/c18c83c4e596b6b031a581cb8e3da73d2ec8b3af7e241a939e28e1cd5bd8/blis-0.7.9-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3dbb44311029263a6f65ed55a35f970aeb1d20b18bfac4c025de5aadf7889a8c"},
+    {url = "https://files.pythonhosted.org/packages/fd/0f/4ec21aeab158b1394215897f08ea3714e3cf8597881a9a261dcf4c471a2d/blis-0.7.9-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:7417667c221e29fe8662c3b2ff9bc201c6a5214bbb5eb6cc290484868802258d"},
+    {url = "https://files.pythonhosted.org/packages/ff/a1/0ece7b0cceda6ca764ecba21e32f099cebff3448d88aa33ff0fce708d34b/blis-0.7.9.tar.gz", hash = "sha256:29ef4c25007785a90ffc2f0ab3d3bd3b75cd2d7856a9a482b7d0dac8d511a09d"},
+]
 "brotab 1.4.2" = [
     {url = "https://files.pythonhosted.org/packages/4e/80/11e6b3b3c2e69654c0f3ac5af03f1f862c920c2b0b246146bf10a755cbe7/brotab-1.4.2-py3-none-any.whl", hash = "sha256:39bc41b2e03e2636f6cd169a68d7db8cf0c1cbc8a9e69e7da9e4c0ca4ebfaab6"},
     {url = "https://files.pythonhosted.org/packages/c8/0b/b01f469f006004aa1294f5d3e2863d4bffd547821281de6d808171c2c59f/brotab-1.4.2.tar.gz", hash = "sha256:07409071eae12ce574872c60cd5a658e6e7f48f0cc9a1b396decdc7689fec7d3"},
 ]
 "brotli 1.0.9" = [
     {url = "https://files.pythonhosted.org/packages/00/7f/6d3405fbbd6883bca364e1d2b8ddbd0617bf063f35bed2c912f8fc723cc2/Brotli-1.0.9-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b1375b5d17d6145c798661b67e4ae9d5496920d9265e2f00f1c2c0b5ae91fbde"},
     {url = "https://files.pythonhosted.org/packages/02/f6/743a4364e89c4942edfe28127ba62ae09d720558d624ce10120342b391bc/Brotli-1.0.9-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:cab1b5964b39607a66adbba01f1c12df2e55ac36c81ec6ed44f2fca44178bf1a"},
@@ -1394,14 +1607,18 @@
     {url = "https://files.pythonhosted.org/packages/cc/17/9418f28b83c85c0108d8b1822359c22ab09f1ec54d3280d742e56645148c/brotlicffi-1.0.9.2-pp36-pypy36_pp73-win32.whl", hash = "sha256:916b790f967a18a595e61f218c252f83718ac91f24157d622cf0fa710cd26ab7"},
     {url = "https://files.pythonhosted.org/packages/d3/d8/6acbb65e350213ad6bd96180593fad0a269a3baa845c67fed21adee3959d/brotlicffi-1.0.9.2.tar.gz", hash = "sha256:0c248a68129d8fc6a217767406c731e498c3e19a7be05ea0a90c3c86637b7d96"},
 ]
 "casttube 0.2.1" = [
     {url = "https://files.pythonhosted.org/packages/0a/d2/0f5006892e07ea342d57dbeda46027e99a097ffb6218bee1e37f9776ed95/casttube-0.2.1-py3-none-any.whl", hash = "sha256:36f118007f9eead3959cf30de03c1640b53a263569ff2a3971c0521826c835b2"},
     {url = "https://files.pythonhosted.org/packages/78/54/f7e80d701c587940cf1c871fb6327b4a2682df4287896fbf9400cd0bbf21/casttube-0.2.1.tar.gz", hash = "sha256:54d2af8c7949aa9c5db87fb11ef0a478a5d3e7ac6d2d2ac8dd1711e3a516fc82"},
 ]
+"catalogue 2.0.8" = [
+    {url = "https://files.pythonhosted.org/packages/dc/28/a2b0cc4bfa7916ef9caf08475be5810fc564411c5a801f225a1f40a458c5/catalogue-2.0.8-py3-none-any.whl", hash = "sha256:2d786e229d8d202b4f8a2a059858e45a2331201d831e39746732daa704b99f69"},
+    {url = "https://files.pythonhosted.org/packages/e5/32/7c208d19bff7fb7147dcf0eb2f5adc54365ea6fc1153201360e031a00b2e/catalogue-2.0.8.tar.gz", hash = "sha256:b325c77659208bfb6af1b0d93b1a1aa4112e1bb29a4c5ced816758a722f0e388"},
+]
 "catt 0.12.11" = [
     {url = "https://files.pythonhosted.org/packages/3d/f7/def2a94aacaedbaf5f755a09acba713b895eaec1cff33df71569f7148f44/catt-0.12.11.tar.gz", hash = "sha256:d1ba9861f5b017bc98a006e364f862fdfe022dc2fcf6299619868c8b907086d7"},
     {url = "https://files.pythonhosted.org/packages/62/17/604bfe5fefb961528ee364cdaf77da2fe634938436d93a3050c2f21e9fa9/catt-0.12.11-py3-none-any.whl", hash = "sha256:db2808d0e344381cb2a1fd8729416ef8b926fb3d5f5507b0f4697a79b095731f"},
 ]
 "certifi 2023.5.7" = [
     {url = "https://files.pythonhosted.org/packages/93/71/752f7a4dd4c20d6b12341ed1732368546bc0ca9866139fe812f6009d9ac7/certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
     {url = "https://files.pythonhosted.org/packages/9d/19/59961b522e6757f0c9097e4493fa906031b95b3ebe9360b2c3083561a6b4/certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
@@ -1568,66 +1785,101 @@
 "colorama 0.4.6" = [
     {url = "https://files.pythonhosted.org/packages/d1/d6/3965ed04c63042e047cb6a3e6ed1a63a35087b6a609aa3a15ed8ac56c221/colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {url = "https://files.pythonhosted.org/packages/d8/53/6f443c9a4a8358a93a6792e2acffb9d9d5cb0a5cfd8802644b7b1c9a02e4/colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 "compressed-rtf 1.0.6" = [
     {url = "https://files.pythonhosted.org/packages/8e/ac/abb196bb0b42a239d605fe97c314c3312374749013a07da4e6e0408f223c/compressed_rtf-1.0.6.tar.gz", hash = "sha256:c1c827f1d124d24608981a56e8b8691eb1f2a69a78ccad6440e7d92fde1781dd"},
 ]
-"cython 0.29.34" = [
-    {url = "https://files.pythonhosted.org/packages/01/7f/be6a89dee727050bc617031ae8a485c01cbf8c52399d638cfbad035ecb6b/Cython-0.29.34-cp35-cp35m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:fd1ea21f1cebf33ae288caa0f3e9b5563a709f4df8925d53bad99be693fc0d9b"},
-    {url = "https://files.pythonhosted.org/packages/04/ef/2b65cdacdd9f327d672af2a37a2c75e8d7e4aeaff6c7a445ba305f1b572f/Cython-0.29.34-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:0e9032cd650b0cb1d2c2ef2623f5714c14d14c28d7647d589c3eeed0baf7428e"},
-    {url = "https://files.pythonhosted.org/packages/0a/70/1500f05bddb16d795b29fac42954b3c8764c82367b8326c10f038471ae7f/Cython-0.29.34.tar.gz", hash = "sha256:1909688f5d7b521a60c396d20bba9e47a1b2d2784bfb085401e1e1e7d29a29a8"},
-    {url = "https://files.pythonhosted.org/packages/18/0d/1ef8b236b029c1bb3b04ba2b7cc167d3b84ad60eba0d2d3241fcecf208a9/Cython-0.29.34-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:a8ad755f9364e720f10a36734a1c7a5ced5c679446718b589259261438a517c9"},
-    {url = "https://files.pythonhosted.org/packages/1b/1c/2cd8a6b8cf8d1e9d1379e3b90e84c739309f74e947ec32b8287147c7950d/Cython-0.29.34-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:dbd79221869ee9a6ccc4953b2c8838bb6ae08ab4d50ea4b60d7894f03739417b"},
-    {url = "https://files.pythonhosted.org/packages/23/08/d301e2e6fd836df6e838e92a244ccef5f1e041d284b8e0a613f4f1294147/Cython-0.29.34-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:1d6c809e2f9ce5950bbc52a1d2352ef3d4fc56186b64cb0d50c8c5a3c1d17661"},
-    {url = "https://files.pythonhosted.org/packages/28/83/6c1f92db53d1242a3ef3ba2d478875b6966dee22cc49cd83bc2ae845aae2/Cython-0.29.34-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:9489de5b2044dcdfd9d6ca8242a02d560137b3c41b1f5ae1c4f6707d66d6e44d"},
-    {url = "https://files.pythonhosted.org/packages/2c/7d/5bc25cbe8ef8680abcdbd019002dcf622b6f2060c95a5abf88b54d8b28e5/Cython-0.29.34-cp35-cp35m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:a0f4229df10bc4545ebbeaaf96ebb706011d8b333e54ed202beb03f2bee0a50e"},
-    {url = "https://files.pythonhosted.org/packages/2f/6d/7dc0e08b5305ffb790043535460c2bf2e1d2a74e46e1e284d0886c6cb0ed/Cython-0.29.34-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:cfb2302ef617d647ee590a4c0a00ba3c2da05f301dcefe7721125565d2e51351"},
-    {url = "https://files.pythonhosted.org/packages/42/e2/85ef37e984213c0867ca767846c61095d802cd5686ee338aaf8ea7354e94/Cython-0.29.34-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:7595d29eaee95633dd8060f50f0e54b27472d01587659557ebcfe39da3ea946b"},
-    {url = "https://files.pythonhosted.org/packages/48/3f/146ae10a3a541b42bc07e7a92af1ca7bf10c3aa05f564616d5b7545b2132/Cython-0.29.34-cp27-cp27mu-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:5a8de3e793a576e40ca9b4f5518610cd416273c7dc5e254115656b6e4ec70663"},
-    {url = "https://files.pythonhosted.org/packages/48/49/e06a169507f7bf43e5c3b3cb5e72cc363d898e86f25fa39f8968ed028147/Cython-0.29.34-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:0963266dad685812c1dbb758fcd4de78290e3adc7db271c8664dcde27380b13e"},
-    {url = "https://files.pythonhosted.org/packages/4b/55/5d131b9f3d4f687e716b402c00eefccf2d0edeab556efe0a3c17bbbce305/Cython-0.29.34-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:459994d1de0f99bb18fad9f2325f760c4b392b1324aef37bcc1cd94922dfce41"},
-    {url = "https://files.pythonhosted.org/packages/51/f0/76f99a049ca056459883b24c3265a82fda3e2093eef71b15717d7e2b75b3/Cython-0.29.34-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:56866323f1660cecb4d5ff3a1fba92a56b91b7cfae0a8253777aa4bdb3bdf9a8"},
-    {url = "https://files.pythonhosted.org/packages/53/97/118cd8e28787496e855f3f08641a91f9a7e94f33f986b1f0aa4a0ececa14/Cython-0.29.34-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:e971db8aeb12e7c0697cefafe65eefcc33ff1224ae3d8c7f83346cbc42c6c270"},
-    {url = "https://files.pythonhosted.org/packages/59/9f/58b57f086f1834a91756227de37dd96ff101b06e24c35957346803b87c6c/Cython-0.29.34-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:f674ceb5f722d364395f180fbac273072fc1a266aab924acc9cfd5afc645aae1"},
-    {url = "https://files.pythonhosted.org/packages/65/7b/170c1f941cdca31c13fba756c48628c707100ac3dc3033b12a7fdc92f99f/Cython-0.29.34-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:44733366f1604b0c327613b6918469284878d2f5084297d10d26072fc6948d51"},
-    {url = "https://files.pythonhosted.org/packages/68/65/8acfd6018b98d0ea7a9b62f3126a73408a540857efbb3bbaf00b12b84162/Cython-0.29.34-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:e4401270b0dc464c23671e2e9d52a60985f988318febaf51b047190e855bbe7d"},
-    {url = "https://files.pythonhosted.org/packages/6a/a0/2708e27d98d557a00b8ea7dc6c2a6c64c115508fda955234462ad3ee41eb/Cython-0.29.34-cp27-cp27mu-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:60969d38e6a456a67e7ef8ae20668eff54e32ba439d4068ccf2854a44275a30f"},
-    {url = "https://files.pythonhosted.org/packages/6b/b8/5250d189bf221d9902092c4ac4dd0a5c16ba5eb7dff4e2d2ec7b76ef4543/Cython-0.29.34-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:8c3cd8bb8e880a3346f5685601004d96e0a2221e73edcaeea57ea848618b4ac6"},
-    {url = "https://files.pythonhosted.org/packages/6f/23/24664adeb330fc0048e9cee5321a23b2902ed3f5493b3fd27d7f84143f06/Cython-0.29.34-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:308c8f1e58bf5e6e8a1c4dcf8abbd2d13d0f9b1e582f4d9ae8b89857342d8bb5"},
-    {url = "https://files.pythonhosted.org/packages/71/1b/1fdf8d92c025435a1097ddff2a2470a761a607a0e62a341ff8c413684e1a/Cython-0.29.34-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:d7ef5f68f4c5baa93349ea54a352f8716d18bee9a37f3e93eff38a5d4e9b7262"},
-    {url = "https://files.pythonhosted.org/packages/78/fe/3fad1d0583e98885dfd1d679fa42923a49c8f51924ffafb25f4f684148fb/Cython-0.29.34-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:21b88200620d80cfe193d199b259cdad2b9af56f916f0f7f474b5a3631ca0caa"},
-    {url = "https://files.pythonhosted.org/packages/8c/d0/5faddf9834eda4d6e040b04730078a5cd24f134a988c8b4ccca860df5f22/Cython-0.29.34-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:7879992487d9060a61393eeefe00d299210256928dce44d887b6be313d342bac"},
-    {url = "https://files.pythonhosted.org/packages/90/4d/05a7e57fca50e527abc52160e3708c14ac67a16384db3e26046f0d5c5c99/Cython-0.29.34-cp27-cp27m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:742544024ddb74314e2d597accdb747ed76bd126e61fcf49940a5b5be0a8f381"},
-    {url = "https://files.pythonhosted.org/packages/96/28/c8815bb3aa85155dd39e0c717cf7816996c4587092417765073dc5ca9da0/Cython-0.29.34-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:5718319a01489688fdd22ddebb8e2fcbbd60be5f30de4336ea7063c3ae29fbe5"},
-    {url = "https://files.pythonhosted.org/packages/a0/85/8aad1a805e669b978c7e969209a9ce42d6776845f2ca47ec71b58f24e229/Cython-0.29.34-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:67b850cf46b861bc27226d31e1d87c0e69869a02f8d3cc5d5bef549764029879"},
-    {url = "https://files.pythonhosted.org/packages/a2/a6/9577ec50401b10ada1603cb7caab62e260934dac0e49fbd52c4ba77b48d9/Cython-0.29.34-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:dce0a36d163c05ae8b21200059511217d79b47baf2b7b0f926e8367bd7a3cc24"},
-    {url = "https://files.pythonhosted.org/packages/b3/4e/5ca633f3cdac081118d63e38afb7e1168384e5f3cc967cfe231078369fc4/Cython-0.29.34-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:e6ef7879668214d80ea3914c17e7d4e1ebf4242e0dd4dabe95ca5ccbe75589a5"},
-    {url = "https://files.pythonhosted.org/packages/b6/db/4a94a698e5246f40bd355525a12cbc536936e816446362feb69d7ed98994/Cython-0.29.34-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:5c121dc185040f4333bfded68963b4529698e1b6d994da56be32c97a90c896b6"},
-    {url = "https://files.pythonhosted.org/packages/b8/a6/8202af91cf8aa2e6b024d9d17d887f228d4173ae0101af9d25adff26cb70/Cython-0.29.34-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:11b1b278b8edef215caaa5250ad65a10023bfa0b5a93c776552248fc6f60098d"},
-    {url = "https://files.pythonhosted.org/packages/c1/f9/806de0ab488bf80317c19576799fc8242b3b7e91b72f080c4dafd0a6a091/Cython-0.29.34-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:e40cf86aadc29ecd1cb6de67b0d9488705865deea4fc185c7ad56d7a6fc78703"},
-    {url = "https://files.pythonhosted.org/packages/c2/91/fe73ac80359215b7887cc32fe873f210a0fdd8c334015ad154cb333e7d3d/Cython-0.29.34-cp27-cp27m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:03daae07f8cbf797506446adae512c3dd86e7f27a62a541fa1ee254baf43e32c"},
-    {url = "https://files.pythonhosted.org/packages/c3/20/152740fdc426f4a52b5615ec69b43dd1823fccee2cca2af28c12b37f0590/Cython-0.29.34-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:0ab3cbf3d62b0354631a45dc93cfcdf79098663b1c65a6033af4a452b52217a7"},
-    {url = "https://files.pythonhosted.org/packages/c4/97/4bc6ac2c2334ff039c23a9f2aa99f70b7d07fa0a995a53c6d018a254cd4f/Cython-0.29.34-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:bdb3285660e3068438791ace7dd7b1efd6b442a10b5c8d7a4f0c9d184d08c8ed"},
-    {url = "https://files.pythonhosted.org/packages/d2/49/9845f14b6716614c832535b67e3b491434d7fdecf510fcb6fe254f60a974/Cython-0.29.34-py2.py3-none-any.whl", hash = "sha256:be4f6b7be75a201c290c8611c0978549c60353890204573078e865423dbe3c83"},
-    {url = "https://files.pythonhosted.org/packages/e5/d6/82f3ec9c36b52d8ebb17067c32b7995f4c2bff450adc5b09536a0bde0d93/Cython-0.29.34-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:d8f822fb6ecd5d88c42136561f82960612421154fc5bf23c57103a367bb91356"},
-    {url = "https://files.pythonhosted.org/packages/e6/e2/97bca65d197f06e31d06dea74509c560a64f5f7cd20ef089dfe12c54cd08/Cython-0.29.34-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:4a2723447d1334484681d5aede34184f2da66317891f94b80e693a2f96a8f1a7"},
-    {url = "https://files.pythonhosted.org/packages/f4/b1/f29d7c8f7aa68bf3c03bd593bc00abd80236f59fd02f4cc3bf980a51e036/Cython-0.29.34-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:b6149f7cc5b31bccb158c5b968e5a8d374fdc629792e7b928a9b66e08b03fca5"},
-    {url = "https://files.pythonhosted.org/packages/f8/77/1d4e1487d93aaabfc696b733abe12f91cb3dac3d6fec2f53efb946ed7fc4/Cython-0.29.34-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:ccb223b5f0fd95d8d27561efc0c14502c0945f1a32274835831efa5d5baddfc1"},
+"confection 0.0.4" = [
+    {url = "https://files.pythonhosted.org/packages/35/03/540079384d9665d752631724f578505ddf721b11a7d8318b964397a7a3b8/confection-0.0.4.tar.gz", hash = "sha256:b1ddf5885da635f0e260a40b339730806dfb1bd17d30e08764f35af841b04ecf"},
+    {url = "https://files.pythonhosted.org/packages/b1/c4/07291f4947d20f545eee76ef20d1eacfb1f80d1d6ab4792bfa6797e0578c/confection-0.0.4-py3-none-any.whl", hash = "sha256:aeac5919ba770c7b281aa5863bb6b0efed42568a7ad8ea26b6cb632154503fb2"},
+]
+"cymem 2.0.7" = [
+    {url = "https://files.pythonhosted.org/packages/00/bd/0369d6325ef95eb71d251720e0f7551727a270b41bacc09db5323b87343c/cymem-2.0.7-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a2971b7da5aa2e65d8fbbe9f2acfc19ff8e73f1896e3d6e1223cc9bf275a0207"},
+    {url = "https://files.pythonhosted.org/packages/01/2f/9d841b40404978d93d0e6c091614c9df63d91483a3b2f1d0472c22285e67/cymem-2.0.7-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a9525ad563b36dc1e30889d0087a0daa67dd7bb7d3e1530c4b61cd65cc756a5b"},
+    {url = "https://files.pythonhosted.org/packages/03/e1/df8296e47d81e1f9055b9ceba0dc4e89d900380674abeff6d94e069ce4f2/cymem-2.0.7-cp37-cp37m-win_amd64.whl", hash = "sha256:5ea6b027fdad0c3e9a4f1b94d28d213be08c466a60c72c633eb9db76cf30e53a"},
+    {url = "https://files.pythonhosted.org/packages/04/27/66b11887a2542fd03c3632209860ddee5fafee58efc508832a269dfb6959/cymem-2.0.7-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:df543a36e7000808fe0a03d92fd6cd8bf23fa8737c3f7ae791a5386de797bf79"},
+    {url = "https://files.pythonhosted.org/packages/09/a6/c120371eb2370744cc80b07d9cf8fd2f1b69d4cf71ad920f0e238dbd36ca/cymem-2.0.7-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9e5e1b7de7952d89508d07601b9e95b2244e70d7ef60fbc161b3ad68f22815f8"},
+    {url = "https://files.pythonhosted.org/packages/1c/f0/daffeefab3645305057ea97b3d4bfe478c28719a4e6b14cbe6095c0de417/cymem-2.0.7-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6c50794c612801ed8b599cd4af1ed810a0d39011711c8224f93e1153c00e08d1"},
+    {url = "https://files.pythonhosted.org/packages/22/ca/6fe64ed47a76af1ecf59c437b6cc135072a06a3cef2ce62f8d8f38ce3cae/cymem-2.0.7-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:85359ab7b490e6c897c04863704481600bd45188a0e2ca7375eb5db193e13cb7"},
+    {url = "https://files.pythonhosted.org/packages/22/d3/61033b089e59bf7827f3db72da2fb003ec3989ba3543bf149e2aa45f11dd/cymem-2.0.7-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3da89464021fe669932fce1578343fcaf701e47e3206f50d320f4f21e6683ca5"},
+    {url = "https://files.pythonhosted.org/packages/22/d8/3a0c220ff497ad7ca3c77d3d6d2825ace2a2ba0e1be1c50b5fcd567577bd/cymem-2.0.7-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:42aedfd2e77aa0518a24a2a60a2147308903abc8b13c84504af58539c39e52a3"},
+    {url = "https://files.pythonhosted.org/packages/2e/91/9854d0fedbd42db157c9a88269dbfe556faed06666d9b44f6296da85a77f/cymem-2.0.7-cp36-cp36m-win_amd64.whl", hash = "sha256:0ac45088abffbae9b7db2c597f098de51b7e3c1023cb314e55c0f7f08440cf66"},
+    {url = "https://files.pythonhosted.org/packages/45/d1/fcd546003ffbeb15916a15d38263ec2d452248f32a5a876462e39fd326ef/cymem-2.0.7-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:4981fc9182cc1fe54bfedf5f73bfec3ce0c27582d9be71e130c46e35958beef0"},
+    {url = "https://files.pythonhosted.org/packages/5d/47/bd5df7891ce656be8ff14ca9993168f391b389545b76b268f9cee8958412/cymem-2.0.7-cp310-cp310-win_amd64.whl", hash = "sha256:864701e626b65eb2256060564ed8eb034ebb0a8f14ce3fbef337e88352cdee9f"},
+    {url = "https://files.pythonhosted.org/packages/6e/9e/2f18aa8f03c6d7692a2f6c884f4bc8f0ab0ba065786f2a4ba966d3e19ef6/cymem-2.0.7-cp311-cp311-win_amd64.whl", hash = "sha256:10178e402bb512b2686b8c2f41f930111e597237ca8f85cb583ea93822ef798d"},
+    {url = "https://files.pythonhosted.org/packages/78/e1/3f840e321e25b60ce88c138282d0d204b3c2a1fcc07e0e5940ff7c662f70/cymem-2.0.7-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:24b779046484674c054af1e779c68cb224dc9694200ac13b22129d7fb7e99e6d"},
+    {url = "https://files.pythonhosted.org/packages/86/1e/c6f9060c59da4428d819f5917a870dea408da9e6723b190e0da447b9721a/cymem-2.0.7-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2aa33f1dbd7ceda37970e174c38fd1cf106817a261aa58521ba9918156868231"},
+    {url = "https://files.pythonhosted.org/packages/8a/df/dd3cb90cb45fafa41a9b8ace5dfef553d50567a9abfd75eef21efb9fc3e1/cymem-2.0.7-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6f9e63e5ad4ed6ffa21fd8db1c03b05be3fea2f32e32fdace67a840ea2702c3d"},
+    {url = "https://files.pythonhosted.org/packages/90/1e/95094bace76d7c62e08f4e189f0e8d558ac44a78c3efa820db530bf4f37e/cymem-2.0.7-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c183257dc5ab237b664f64156c743e788f562417c74ea58c5a3939fe2d48d6f6"},
+    {url = "https://files.pythonhosted.org/packages/96/99/a5f558006387913f1a1b4af5ccae610b19ebe5498e7199c2da10e77429c8/cymem-2.0.7-cp38-cp38-win_amd64.whl", hash = "sha256:48b98da6b906fe976865263e27734ebc64f972a978a999d447ad6c83334e3f90"},
+    {url = "https://files.pythonhosted.org/packages/b0/d3/50c90dd821e44ad289653f0029d1690fca82f90df293e77e21443f5ea4fc/cymem-2.0.7.tar.gz", hash = "sha256:e6034badb5dd4e10344211c81f16505a55553a7164adc314c75bd80cf07e57a8"},
+    {url = "https://files.pythonhosted.org/packages/b1/62/c615d7ff20647b1c568eac00a94df1e88e7c379646659eb0be6e346cadfe/cymem-2.0.7-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f165d7bce55d6730930e29d8294569788aa127f1be8d1642d9550ed96223cb37"},
+    {url = "https://files.pythonhosted.org/packages/b2/f1/767458d63d2162ce8492f462ad5f92125d3d43eabc3a03bf043e57c3512f/cymem-2.0.7-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:e156788d32ad8f7141330913c5d5d2aa67182fca8f15ae22645e9f379abe8a4c"},
+    {url = "https://files.pythonhosted.org/packages/ca/be/1f6ac43fea9f7c353acf7db81bd01f651887882ce27e8018759949374cef/cymem-2.0.7-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d18250f97eeb13af2e8b19d3cefe4bf743b963d93320b0a2e729771410fd8cf4"},
+    {url = "https://files.pythonhosted.org/packages/cb/6a/3cb5e33ad0adc201eadbdff70be4d54fdc2772947252fc157dc9a041bf16/cymem-2.0.7-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:26e5d5c6958855d2fe3d5629afe85a6aae5531abaa76f4bc21b9abf9caaccdfe"},
+    {url = "https://files.pythonhosted.org/packages/cd/fb/cd73656ffb41a05452ec90bd7a201f1e065310c013efa20269cb80c2531f/cymem-2.0.7-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:011039e12d3144ac1bf3a6b38f5722b817f0d6487c8184e88c891b360b69f533"},
+    {url = "https://files.pythonhosted.org/packages/d5/09/819e5a536f898c8f464da28a74b13b0b56683e307949c62a319a57afb162/cymem-2.0.7-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:314273be1f143da674388e0a125d409e2721fbf669c380ae27c5cbae4011e26d"},
+    {url = "https://files.pythonhosted.org/packages/d8/2d/61953a623544f0b87d931e5393dbe7ca0ea727e87c72ab95db715c8abecb/cymem-2.0.7-cp39-cp39-win_amd64.whl", hash = "sha256:59a09cf0e71b1b88bfa0de544b801585d81d06ea123c1725e7c5da05b7ca0d20"},
+    {url = "https://files.pythonhosted.org/packages/f1/be/8af4c91f3cd7453284733ca66ce2e3ed97f4602adf170b6e3d9b21a89dd3/cymem-2.0.7-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4f359cab9f16e25b3098f816c40acbf1697a3b614a8d02c56e6ebcb9c89a06b3"},
+    {url = "https://files.pythonhosted.org/packages/f7/04/34905a11acdf77f9788790871a2f8b19d2adc7a6f6f4df16f74b601e2866/cymem-2.0.7-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:4302df5793a320c4f4a263c7785d2fa7f29928d72cb83ebeb34d64a610f8d819"},
+]
+"cython 0.29.35" = [
+    {url = "https://files.pythonhosted.org/packages/01/fd/5e489abe8ee99a52366b5ae99518b64f6024c6dd331b4d75a6a9ac48f429/Cython-0.29.35-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:c4cd7de707938b8385cd1f88e1446228fbfe09af7822fa13877a4374c4881198"},
+    {url = "https://files.pythonhosted.org/packages/07/8d/1f1b35002360b356dc0d280271190fdc03d4c359bd59113437ad107608ed/Cython-0.29.35-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:402307ad6fd209816cf539680035ef79cce171288cb98f81f3f11ea8ef3afd99"},
+    {url = "https://files.pythonhosted.org/packages/11/c4/12a69dd2f0bdf56841fefba124ab17e9b9641dbb5515fb9b790a77c72674/Cython-0.29.35-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:e7b1901b03c37a082ba405e2cf73a57091e835c7af35f664f9dd1d855a992ad5"},
+    {url = "https://files.pythonhosted.org/packages/16/d0/4f6f0035231895ea3d7ba5e40f0d11cb2c0f8255e4704631c7c6686a9e3c/Cython-0.29.35-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:537bc1e0ed9bf7289c80f39a9a9359f5649068647631996313f77ba57afde40b"},
+    {url = "https://files.pythonhosted.org/packages/21/6b/b8b310ae37b4b575a5dcc78f390414a0ddac146a27418fec3e533132af3d/Cython-0.29.35-cp35-cp35m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:520c50d1875627c111900d7184fd658e32967a3ef807dc2fbc252e384839cbcf"},
+    {url = "https://files.pythonhosted.org/packages/29/6a/2b815ceba362b6e3f35647f5bb54db1ce35635b3b356ec36f855100ba0cc/Cython-0.29.35-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:3da42ef5b71674e4864b6afbe1bcacba75807684e22b6337f753cf297ae4e2d2"},
+    {url = "https://files.pythonhosted.org/packages/34/75/fc909128c082452a3ebb8030e3adb3c8ed6f2a561183c6e46597aaa6ef0f/Cython-0.29.35-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:511f3adfb2db4db2eb882f892525db18a3a21803830474d2fa8b7a1a0f406985"},
+    {url = "https://files.pythonhosted.org/packages/4d/6e/0af669802b540c7d37afd32e9c467eb5d922ba92a7c039c7b4d13ae08d40/Cython-0.29.35-cp35-cp35m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:516abc754f15b84d6a8e71c8abd90e10346ea86001563480f0be1b349d09c6b8"},
+    {url = "https://files.pythonhosted.org/packages/53/9e/272e0945e4fb3e52411aa088f3ef4ab046569ba6c786263e90ef92aa61b3/Cython-0.29.35-cp27-cp27mu-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:c1d7a9ff809fa9b4a9fe04df86c9f7f574ca31c2ad896462a97ea89523db286a"},
+    {url = "https://files.pythonhosted.org/packages/61/1d/e3111e8ea7d3ed4656d74ec9b4fbecd55844c27dde2fae03fa1f6d7a5c6b/Cython-0.29.35-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:99477c1d4a105a562c05d43cc01905b6711f0a6a558d90f20c7aee0fb23d59d5"},
+    {url = "https://files.pythonhosted.org/packages/66/46/4fdf01790dd9af45c55a850d4f9298d00a4d15dc40c6500482e288893275/Cython-0.29.35-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:05b7ede0b0eb1c6b9bd748fa67c5ebf3c3560d04d7c8a1486183ddd099de5a00"},
+    {url = "https://files.pythonhosted.org/packages/67/11/8536814895e77757f5ad8c45c338c18f0496f2cede6820e4af59a867ac7e/Cython-0.29.35-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:5a47974f3ebccf25702ffdd569904f7807ea1ef0830987c133877fabefdc4bab"},
+    {url = "https://files.pythonhosted.org/packages/6c/6a/4377e6401b791b4ca6f65b29fe6e8974a4428e910ee7f843a47e4d03df0a/Cython-0.29.35-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:563a02ea675ed6321d6257df067c89f17b89a63487ef8b9ce0d598e88e7ff0bd"},
+    {url = "https://files.pythonhosted.org/packages/7b/44/72eba4b4896d9d3275e9694b36070952a94ea31744384898f75287242308/Cython-0.29.35-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:a1ad51612ff6cfe05cd58f584f01373d64906bb0c860a067c6441359ff10464f"},
+    {url = "https://files.pythonhosted.org/packages/81/37/dac865bb0e02643428a61c33934bb0052bdd18847f810fcbbd8f8001300c/Cython-0.29.35-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:c17c876db737e1183d18d23db9cc31a9f565c113a32523c672af72f6497e382f"},
+    {url = "https://files.pythonhosted.org/packages/85/03/b21dda87f7b3d5f0ef2eceff78e085770a0b98c3642ab65f54d3758bcf92/Cython-0.29.35-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:94859c3fd90767995b33d803edecad21e73749823db468d34f21e80451a11a99"},
+    {url = "https://files.pythonhosted.org/packages/8f/6a/6ad26c864debaa3e4fadfdd98374af1422cd2efa9d72263e3ce5fc9c3b33/Cython-0.29.35-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:ea1c166336188630cd3e48aea4bbe06ea1bab444624e31c78973fffcae1cf708"},
+    {url = "https://files.pythonhosted.org/packages/8f/fd/6a48390d1c7dab5eb174729c37ba1e7ad27c8d2982cef23354131fa313a5/Cython-0.29.35-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:8841158f274896702afe732571d37be22868a301275f952f6280547b25280538"},
+    {url = "https://files.pythonhosted.org/packages/90/eb/f3dae8f04ead83827b94618c48e946639cd68d21cabeeb92ee22bbad8265/Cython-0.29.35-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:2e1e5d62f15ea4fa4a8bc76e4fcc2ea313a8afe70488b7b870716bcfb12b8246"},
+    {url = "https://files.pythonhosted.org/packages/93/ba/8b47280fa9738bcf63a59d36b374839dd11127712036d6d55431860dd42f/Cython-0.29.35-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:c44bb47b314abc743705c7d038d351ffc3a34b95ab59b04b8cb27cf781b44ae8"},
+    {url = "https://files.pythonhosted.org/packages/9b/bd/4d9f5a4d1ca6c991e0bd26c6ca646eed8fc17e0109516cc8170c2dba1319/Cython-0.29.35-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:75541567a2de1f893d247a7f9aa300dff5662fb33822a5fb75bc9621369b8ef0"},
+    {url = "https://files.pythonhosted.org/packages/a3/36/ebb1e780b7364e239bc41348cf2e644f5b7192232bea76d7f7c124de87dc/Cython-0.29.35-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:c38e2c1e94b596132454b29757536d5afa810011d8bcb86918cc6693d2302940"},
+    {url = "https://files.pythonhosted.org/packages/ac/9a/bd7a00981e87e4cc55104d9560feaa794d913486f8a843ff2bdb3e460f7c/Cython-0.29.35-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:ef2fc6f81aa8fb512535b01199fbe0d0ecafb8a29f261055e4b3f103c7bd6c75"},
+    {url = "https://files.pythonhosted.org/packages/ae/d8/89c720a980afbbc694f3ca07456a773e8002d8679977acd318a3b9e4990a/Cython-0.29.35-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:5cdd65f7d85e15f1662c75d85d837c20d5c68acdd1029bfd08fb44c4422d7d9b"},
+    {url = "https://files.pythonhosted.org/packages/b0/98/71c4757e03b2e36f409075841a518c2bd5c7e88618692fd6de5f2a8b0c4f/Cython-0.29.35-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:247d585d8e49f002e522f3420751a4b3da0cf8532ef64d382e0bc9b4c840642c"},
+    {url = "https://files.pythonhosted.org/packages/b1/b6/e9da7005030cd7d6b15c243b69463978717a8b1fb79b29107966760741f2/Cython-0.29.35-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:3cd717eee52072be8244bb07f0e4126f893214d2dfd1ba8b38b533e1ffec4f8a"},
+    {url = "https://files.pythonhosted.org/packages/c8/11/f86cfdf768b5abaff5bdbe8a14a348be6a92180c4600ffef48d50340a0c5/Cython-0.29.35-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:acab11c834cbe8fb7b71f9f7b4c4655afd82ffadb1be93d5354a67702fcee69d"},
+    {url = "https://files.pythonhosted.org/packages/cd/3f/4b1cfc3b1692fa5d4478f88426a84860d8f34d9b5b48c014322c4d1c1bf5/Cython-0.29.35-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:445e092708c26b357c97b3c68ea3eab31846fc9c1360bb150225f340c20322ec"},
+    {url = "https://files.pythonhosted.org/packages/d3/f6/f2c540ed76fa03f76bcc64d3fc730520a7be55ca9cc399cda610a5bcd9d1/Cython-0.29.35-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:156ae92bedcd8261b5259724e2dc4d8eb12ac29159359e34c8358b65d24430ac"},
+    {url = "https://files.pythonhosted.org/packages/d5/57/ce6fcdf9a553e60ff0609870b02c02b99f3811bfb457a66a7f800d792974/Cython-0.29.35-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:0a9334d137bd42fca34b6b413063e19c194ba760846f34804ea1fb477cbe9a88"},
+    {url = "https://files.pythonhosted.org/packages/d6/2b/ab2edcf60504560e5555e0599ea8e06550249f0bbfbc4691a58473a90682/Cython-0.29.35-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:2a2f2fb9b1c0a4a3890713127fba55a38d2cf1619b2570c43c92a93fee80111a"},
+    {url = "https://files.pythonhosted.org/packages/d9/da/5ef847a8c2ad70e648e83b23a6f6cae3fe41d9c3ea231811f393f3416486/Cython-0.29.35-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:27f58d0dd53a8ffb614814c725d3ee3f136e53178611f7f769ff358f69e50502"},
+    {url = "https://files.pythonhosted.org/packages/da/a0/298340fb8412574a0b00a0d9856aa27e7038da429b9e31d6825173d1e6bd/Cython-0.29.35.tar.gz", hash = "sha256:6e381fa0bf08b3c26ec2f616b19ae852c06f5750f4290118bf986b6f85c8c527"},
+    {url = "https://files.pythonhosted.org/packages/e0/ce/a986b79a760dda37deeefa2cb3d914dcba16dd9b0ce4f560fd13b5e15b15/Cython-0.29.35-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:b63ea04db03190dc8b25d167598989be5c1fe9fc3121d7802c0aafc8a4ec383f"},
+    {url = "https://files.pythonhosted.org/packages/e4/3c/9fd5f5d5315e965bce8fbb8679dcc9d86ec51700a03fbaabf6271bfd171f/Cython-0.29.35-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:6c19e2ba027d2e9e2d88a08aa6007344be781ed99bc0924deb237ec52ca14c09"},
+    {url = "https://files.pythonhosted.org/packages/e9/79/c586afabee294dc4bca80e06b0f26d91131fef34bfd480779f0506c51450/Cython-0.29.35-cp27-cp27mu-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:ba534e07543b44fb5ae37e56e61072ed1021b2d6ed643dbb92afa8239a04aa83"},
+    {url = "https://files.pythonhosted.org/packages/ec/da/e03464c39b590fffbf4c984c180320aebc439bbe9171db98b1618efb7b42/Cython-0.29.35-cp27-cp27m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:9e54b4bee55fec952333126147b89c195ebe1d60e8e492ec778916ca5ca03151"},
+    {url = "https://files.pythonhosted.org/packages/ef/30/90dd6a7e4bfa8ccb617ce236978fce26fe9e77ee7783309aa5c2aaba7d92/Cython-0.29.35-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:db695a19968a54b9ac53048c723234b4f0db7409def0a5c5517237202e7a9b92"},
+    {url = "https://files.pythonhosted.org/packages/ef/c6/c073f91693ea355ec1d8ef100156bfbd204614922edc4e41a87ba854b883/Cython-0.29.35-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl", hash = "sha256:be7e1f98a359408186025f84d28d243e4527acb976f06b8ae8441dc5db204280"},
+    {url = "https://files.pythonhosted.org/packages/f2/01/e4e0c2c3fd528f0bfd7fc63edeb7b361cb4789fe173eb63feb5b398cf067/Cython-0.29.35-py2.py3-none-any.whl", hash = "sha256:417703dc67c447089258ab4b3d217f9c03894574e4a0d6c50648a208bc8352bb"},
+    {url = "https://files.pythonhosted.org/packages/f6/ee/9205eeaf3a747142f6e88f2e1e5e9fe3a5aa9458c86e9f48f0b3b19e24f3/Cython-0.29.35-cp27-cp27m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:fb8c11cd3e2d5ab7c2da78c5698e527ecbe469437326811562a3fbf4c5780ae4"},
 ]
 "decorator 5.1.1" = [
     {url = "https://files.pythonhosted.org/packages/66/0c/8d907af351aa16b42caae42f9d6aa37b900c67308052d10fdce809f8d952/decorator-5.1.1.tar.gz", hash = "sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330"},
     {url = "https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl", hash = "sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186"},
 ]
 "docx2txt 0.8" = [
     {url = "https://files.pythonhosted.org/packages/7d/7d/60ee3f2b16d9bfdfa72e8599470a2c1a5b759cb113c6fe1006be28359327/docx2txt-0.8.tar.gz", hash = "sha256:2c06d98d7cfe2d3947e5760a57d924e3ff07745b379c8737723922e7009236e5"},
 ]
-"dogpile-cache 1.2.0" = [
-    {url = "https://files.pythonhosted.org/packages/01/bc/c6ff56c73fb4d9859a0f3080ed5d454646d6849e8a9aede1f95cb2771de4/dogpile.cache-1.2.0.tar.gz", hash = "sha256:47554c860ceb484dd5aef9ff1f88fecb3d4aef6bb92119450f5bcbaa026bbfb1"},
-    {url = "https://files.pythonhosted.org/packages/08/4f/11c49c820186a436471d5c15075456621a0bcd710dac7bac5e7b62e3bbcb/dogpile.cache-1.2.0-py3-none-any.whl", hash = "sha256:d371f310bcdbe5d9c8e7e473348b75c5c97517ac8be16759b24dbaadef1c70a6"},
+"dogpile-cache 1.2.1" = [
+    {url = "https://files.pythonhosted.org/packages/21/fa/2fec52e38feb6ce89930be010314aa99ff616d6f6dc068cfaa7491ce5f3e/dogpile.cache-1.2.1.tar.gz", hash = "sha256:1d0be0cef90505c9f24e9f00aedab8dce9356d28a4153d5660ab13eeb6a0cfd4"},
+    {url = "https://files.pythonhosted.org/packages/37/b3/d95ba629fa9d52cc2ea86298d930976f1e6a560d20fec64527342e61e29e/dogpile.cache-1.2.1-py3-none-any.whl", hash = "sha256:fa9c9c07640bdb66c5f5574e308123119b96c9a95c6856151d3fd2c91b4fb06a"},
 ]
 "ebcdic 1.1.1" = [
     {url = "https://files.pythonhosted.org/packages/0d/2f/633031205333bee5f9f93761af8268746aa75f38754823aabb8570eb245b/ebcdic-1.1.1-py2.py3-none-any.whl", hash = "sha256:33b4cb729bc2d0bf46cc1847b0e5946897cb8d3f53520c5b9aa5fa98d7e735f1"},
 ]
 "enzyme 0.4.1" = [
     {url = "https://files.pythonhosted.org/packages/dd/99/e4eee822d9390ebf1f63a7a67e8351c09fb7cd75262e5bb1a5256898def9/enzyme-0.4.1.tar.gz", hash = "sha256:f2167fa97c24d1103a94d4bf4eb20f00ca76c38a37499821049253b2059c62bb"},
 ]
@@ -1730,17 +1982,17 @@
 "ftfy 6.1.1" = [
     {url = "https://files.pythonhosted.org/packages/97/16/79c6e17bd3465f6498282dd23813846c68cd0989fe60bfef68bb1918d041/ftfy-6.1.1.tar.gz", hash = "sha256:bfc2019f84fcd851419152320a6375604a0f1459c281b5b199b2cd0d2e727f8f"},
     {url = "https://files.pythonhosted.org/packages/e1/1e/bf736f9576a8979752b826b75cbd83663ff86634ea3055a766e2d8ad3ee5/ftfy-6.1.1-py3-none-any.whl", hash = "sha256:0ffd33fce16b54cccaec78d6ec73d95ad370e5df5a25255c8966a6147bd667ca"},
 ]
 "future 0.18.3" = [
     {url = "https://files.pythonhosted.org/packages/8f/2e/cf6accf7415237d6faeeebdc7832023c90e0282aa16fd3263db0eb4715ec/future-0.18.3.tar.gz", hash = "sha256:34a17436ed1e96697a86f9de3d15a3b0be01d8bc8de9c1dffd59fb8234ed5307"},
 ]
-"gallery-dl 1.25.4" = [
-    {url = "https://files.pythonhosted.org/packages/18/fc/a4af2c1e8de06c46464d67b3cf3993914d9a9b1ce1d6e3840ae82a90f09b/gallery_dl-1.25.4.tar.gz", hash = "sha256:e31d178d7ae21002564a66c68c15b16795895bdaee184f7056b7596137bac04e"},
-    {url = "https://files.pythonhosted.org/packages/4a/03/52dc3552087349a63eb94b6b9c6591205284ba9f93c9b999fb08f3b57146/gallery_dl-1.25.4-py3-none-any.whl", hash = "sha256:62396d46abe38c7f14c27e86734b14bcec9c395a76eb02a40a46f66cf6238fe2"},
+"gallery-dl 1.25.5" = [
+    {url = "https://files.pythonhosted.org/packages/77/f6/f62a94277168fd5f2adbed55f2358250b0aa3eb9508847fedb73090e842d/gallery_dl-1.25.5.tar.gz", hash = "sha256:205cca54722e659d962e4db766acb1bf0c57178e5fd8efd502a43f8fdf31e1a8"},
+    {url = "https://files.pythonhosted.org/packages/aa/d9/f9e4e2f7722c2b4c27fab9431c85b2e7f40c870d0537955073e548ea2ddf/gallery_dl-1.25.5-py3-none-any.whl", hash = "sha256:9b2c7f16954eeceeb8ede1f88f5e7b6bd13ebc680d54b5e8fee8e997d587e930"},
 ]
 "guessit 3.7.1" = [
     {url = "https://files.pythonhosted.org/packages/96/5f/64304acee35bac703cee51656a5caf37bd18c9490561fbff225922f41d39/guessit-3.7.1.tar.gz", hash = "sha256:2c18d982ee6db30db5d59557add0324a2b49bf3940a752947510632a2b58a3c1"},
     {url = "https://files.pythonhosted.org/packages/db/5e/eec6416047845a745b1d2aee181244b380e59158e29d814021d2e511b267/guessit-3.7.1-py3-none-any.whl", hash = "sha256:c3be280ee8ec581a45ca6a654a92e317bf89567fdc55e7167452226f4f5b8b38"},
 ]
 "humanize 4.6.0" = [
     {url = "https://files.pythonhosted.org/packages/06/b1/9e491df2ee1c919d67ee328d8bc9f17b7a9af68e4077f3f5fac83a4488c9/humanize-4.6.0.tar.gz", hash = "sha256:5f1f22bc65911eb1a6ffe7659bd6598e33dcfeeb904eb16ee1e705a09bf75916"},
@@ -1790,14 +2042,18 @@
     {url = "https://files.pythonhosted.org/packages/15/02/afd43c5066de05f6b3188f3aa74136a3289e6c30e7a45f351546cab0928c/jedi-0.18.2.tar.gz", hash = "sha256:bae794c30d07f6d910d32a7048af09b5a39ed740918da923c6b780790ebac612"},
     {url = "https://files.pythonhosted.org/packages/6d/60/4acda63286ef6023515eb914543ba36496b8929cb7af49ecce63afde09c6/jedi-0.18.2-py2.py3-none-any.whl", hash = "sha256:203c1fd9d969ab8f2119ec0a3342e0b49910045abe6af0a3ae83a5764d54639e"},
 ]
 "jinja2 3.1.2" = [
     {url = "https://files.pythonhosted.org/packages/7a/ff/75c28576a1d900e87eb6335b063fab47a8ef3c8b4d88524c4bf78f670cce/Jinja2-3.1.2.tar.gz", hash = "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852"},
     {url = "https://files.pythonhosted.org/packages/bc/c3/f068337a370801f372f2f8f6bad74a5c140f6fda3d9de154052708dd3c65/Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
 ]
+"langcodes 3.3.0" = [
+    {url = "https://files.pythonhosted.org/packages/5f/ec/9955d772ecac0bdfb5d706d64f185ac68bd0d4092acdc2c5a1882c824369/langcodes-3.3.0.tar.gz", hash = "sha256:794d07d5a28781231ac335a1561b8442f8648ca07cd518310aeb45d6f0807ef6"},
+    {url = "https://files.pythonhosted.org/packages/fe/c3/0d04d248624a181e57c2870127dfa8d371973561caf54333c85e8f9133a2/langcodes-3.3.0-py3-none-any.whl", hash = "sha256:4d89fc9acb6e9c8fdef70bcdf376113a3db09b67285d9e1d534de6d8818e7e69"},
+]
 "lxml 4.9.2" = [
     {url = "https://files.pythonhosted.org/packages/00/d9/d2ae5c7032157798df585321fc190b51062eb9970edb017ef15127ac899b/lxml-4.9.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:5344a43228767f53a9df6e5b253f8cdca7dfc7b7aeae52551958192f56d98457"},
     {url = "https://files.pythonhosted.org/packages/06/5a/e11cad7b79f2cf3dd2ff8f81fa8ca667e7591d3d8451768589996b65dec1/lxml-4.9.2.tar.gz", hash = "sha256:2455cfaeb7ac70338b3257f41e21f0724f4b5b0c0e7702da67ee6c3640835b67"},
     {url = "https://files.pythonhosted.org/packages/08/14/bf49d3676262c31343d27f8d2b8553dd0ca62d0d7a7a44faf9d98f52a10b/lxml-4.9.2-pp37-pypy37_pp73-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:b264171e3143d842ded311b7dccd46ff9ef34247129ff5bf5066123c55c2431c"},
     {url = "https://files.pythonhosted.org/packages/0a/69/4e78395c575852fcccb493203b4ac5923f18c8503fcc2cb232a27828d3ca/lxml-4.9.2-cp36-cp36m-win32.whl", hash = "sha256:d5bf6545cd27aaa8a13033ce56354ed9e25ab0e4ac3b5392b763d8d04b08e0c5"},
     {url = "https://files.pythonhosted.org/packages/12/88/9b4be59b4e9d99762bb6301ee712202eaafc79b6db46fba613e854419759/lxml-4.9.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:7d2278d59425777cfcb19735018d897ca8303abe67cc735f9f97177ceff8027f"},
     {url = "https://files.pythonhosted.org/packages/12/fd/5d21bb2d12b5d2a738ee7dd2700c33ebbab0604a356691bebe0a8cd18970/lxml-4.9.2-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:0dc313ef231edf866912e9d8f5a042ddab56c752619e92dfd3a2c277e6a7299a"},
@@ -2013,14 +2269,44 @@
     {url = "https://files.pythonhosted.org/packages/f1/d2/d735d40355ce41f6d1c50a5d4feef47cd4aad0e2809dd2c8cb01601f04ac/multidict-6.0.4-cp39-cp39-win_amd64.whl", hash = "sha256:33029f5734336aa0d4c0384525da0387ef89148dc7191aae00ca5fb23d7aafc2"},
     {url = "https://files.pythonhosted.org/packages/f1/d7/7f26fe2e790654dcc82283c17b69534c7f30213b63628e7420391d609166/multidict-6.0.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:45e1ecb0379bfaab5eef059f50115b54571acfbe422a14f668fc8c27ba410e7e"},
     {url = "https://files.pythonhosted.org/packages/f5/cf/416f84a8c7954c571881b01c839312ec81e222b3986c8baedc57f476cc1b/multidict-6.0.4-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ea20853c6dbbb53ed34cb4d080382169b6f4554d394015f1bef35e881bf83547"},
     {url = "https://files.pythonhosted.org/packages/fc/54/8e025ae4e31d899e4528a570941eb7048512392b454acccf69c2dccfcb0d/multidict-6.0.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:eeb6dcc05e911516ae3d1f207d4b0520d07f54484c49dfc294d6e7d63b734171"},
     {url = "https://files.pythonhosted.org/packages/fc/5b/0a4205a1248fb152f596a03c971c6ef1585d0c98e56b6886dc35d084e366/multidict-6.0.4-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7d18748f2d30f94f498e852c67d61261c643b349b9d2a581131725595c45ec6c"},
     {url = "https://files.pythonhosted.org/packages/fe/0c/8469202f8f4b0e65816f91c3febc4bda7316c995b59ecdf3b15c574f7a24/multidict-6.0.4-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cc8e1d0c705233c5dd0c5e6460fbad7827d5d36f310a0fadfd45cc3029762258"},
 ]
+"murmurhash 1.0.9" = [
+    {url = "https://files.pythonhosted.org/packages/1a/e5/5a831a02def7f67ea69a0bf82f145636308d5ace344061fba79e979a08ce/murmurhash-1.0.9-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:213d0248e586082e1cab6157d9945b846fd2b6be34357ad5ea0d03a1931d82ba"},
+    {url = "https://files.pythonhosted.org/packages/1c/f7/fa4190a6815f1da2ae3fd4624e2a84bb1e9b6cdb74036a38959f78ad5891/murmurhash-1.0.9-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f9b995bc82eaf9223e045210207b8878fdfe099a788dd8abd708d9ee58459a9d"},
+    {url = "https://files.pythonhosted.org/packages/28/08/2d1a72c9aace7631522852937f7720906216a64202aa7a3a34f73a96a786/murmurhash-1.0.9-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d7a2bd203377a31bbb2d83fe3f968756d6c9bbfa36c64c6ebfc3c6494fc680bc"},
+    {url = "https://files.pythonhosted.org/packages/29/02/d67c327bc0690c98a07456b8d4caf6e4b66c42de196a2cf49350fea13de5/murmurhash-1.0.9-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:47f5ca56c430230d3b581dfdbc54eb3ad8b0406dcc9afdd978da2e662c71d370"},
+    {url = "https://files.pythonhosted.org/packages/2b/a6/88a2bcca18ea01a469844d84e666f37607b36e4f0a8946dca03b54428511/murmurhash-1.0.9-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0c2e2ee2d91a87952fe0f80212e86119aa1fd7681f03e6c99b279e50790dc2b3"},
+    {url = "https://files.pythonhosted.org/packages/2c/16/a5223c2e02e6dd908fa0c93056f612ff6af6c639cbff631a380f45279beb/murmurhash-1.0.9-cp38-cp38-win_amd64.whl", hash = "sha256:a5952f9c18a717fa17579e27f57bfa619299546011a8378a8f73e14eece332f6"},
+    {url = "https://files.pythonhosted.org/packages/2e/a9/91f972c49846c967c5c78bb18c40fba3330a4d5ee24f88f4641e4574dbe0/murmurhash-1.0.9-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:0ac5530c250d2b0073ed058555847c8d88d2d00229e483d45658c13b32398523"},
+    {url = "https://files.pythonhosted.org/packages/35/e6/d5717bf4d5babfd8f6dda1c7e55c2b77d3a2d9a1e1449c6dcb8cbe769e7b/murmurhash-1.0.9-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0eb0f8e652431ea238c11bcb671fef5c03aff0544bf7e098df81ea4b6d495405"},
+    {url = "https://files.pythonhosted.org/packages/5f/57/06bd0a336b49520f83db24ca2c1181429d3d0922850a5804a32dfdee1ce7/murmurhash-1.0.9-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:5ef31b5c11be2c064dbbdd0e22ab3effa9ceb5b11ae735295c717c120087dd94"},
+    {url = "https://files.pythonhosted.org/packages/60/ea/380ada3ed5bafd4b1f76903e3dad7cae9bd4659fc7fdd52e0b92c872f8b2/murmurhash-1.0.9-cp310-cp310-win_amd64.whl", hash = "sha256:cf0b3fe54dca598f5b18c9951e70812e070ecb4c0672ad2cc32efde8a33b3df6"},
+    {url = "https://files.pythonhosted.org/packages/75/59/7bbe46ef97680eb5d09342b9964b992b0a55faec4883f6071b53042d1447/murmurhash-1.0.9-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:799fcbca5693ad6a40f565ae6b8e9718e5875a63deddf343825c0f31c32348fa"},
+    {url = "https://files.pythonhosted.org/packages/78/30/73bd92965c6eb74b3dd1ef24b0f0288268b35bdc4ce7588c47b5f4ddb7c0/murmurhash-1.0.9-cp39-cp39-win_amd64.whl", hash = "sha256:379bf6b414bd27dd36772dd1570565a7d69918e980457370838bd514df0d91e9"},
+    {url = "https://files.pythonhosted.org/packages/7c/28/688986202be2bd48066dda362f8299091a595bde930f4785f484bb22c298/murmurhash-1.0.9-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:01137d688a6b259bde642513506b062364ea4e1609f886d9bd095c3ae6da0b94"},
+    {url = "https://files.pythonhosted.org/packages/84/4e/7ce0e1bba5c523999a07c92e269d8061882f65c3117749ee0984f3a3e11c/murmurhash-1.0.9-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:69157e8fa6b25c4383645227069f6a1f8738d32ed2a83558961019ca3ebef56a"},
+    {url = "https://files.pythonhosted.org/packages/8a/4f/9b905a12acfbd431fc9842bf92079ef3511083ef21c31a9a1191f8f25b89/murmurhash-1.0.9-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:94b89d02aeab5e6bad5056f9d08df03ac7cfe06e61ff4b6340feb227fda80ce8"},
+    {url = "https://files.pythonhosted.org/packages/92/2b/6b2dda111246f4133b8911e84aa87c9a70b29fdc944b4d9eeaa9a3448f34/murmurhash-1.0.9-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:241693c1c819148eac29d7882739b1099c891f1f7431127b2652c23f81722cec"},
+    {url = "https://files.pythonhosted.org/packages/99/bb/1ee299085fbbd9062d339967e74f57f8fb2e780bbcc7374265d9ce36d7e2/murmurhash-1.0.9-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:ab78675510f83e7a3c6bd0abdc448a9a2b0b385b0d7ee766cbbfc5cc278a3042"},
+    {url = "https://files.pythonhosted.org/packages/a6/16/f42825d9f521964319f107f38c4fc4c15b47f0a0381726a5be0ca10ec930/murmurhash-1.0.9-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:5dc41be79ba4d09aab7e9110a8a4d4b37b184b63767b1b247411667cdb1057a3"},
+    {url = "https://files.pythonhosted.org/packages/a7/e8/10e30f486baec17513798f71a7677aa78c44758d7e638bfe8fb569ca7fb0/murmurhash-1.0.9-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1b70bbf55d89713873a35bd4002bc231d38e530e1051d57ca5d15f96c01fd778"},
+    {url = "https://files.pythonhosted.org/packages/ba/2d/0e57ce9afb57c25d1f9efea27f7cbeebd728eef074e073e57300d54b55e2/murmurhash-1.0.9-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2aebe2ae016525a662ff772b72a2c9244a673e3215fcd49897f494258b96f3e7"},
+    {url = "https://files.pythonhosted.org/packages/c1/0c/db040fad5ee5a590b00a7e24f9e72db2ce578979ad0493474e6bc304841e/murmurhash-1.0.9-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:ef79202feeac68e83971239169a05fa6514ecc2815ce04c8302076d267870f6e"},
+    {url = "https://files.pythonhosted.org/packages/c1/aa/d2d8b0caaef7aae36a5e856f0c6b736145c57f2b67652b4fccb738ca9bdd/murmurhash-1.0.9-cp311-cp311-win_amd64.whl", hash = "sha256:660ae41fc6609abc05130543011a45b33ca5d8318ae5c70e66bbd351ca936063"},
+    {url = "https://files.pythonhosted.org/packages/ce/4a/139a0f0ed47afc324843357b021233f5cf16e4b28fd0d322f0ec54ee6d0e/murmurhash-1.0.9-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b129e1c5ebd772e6ff5ef925bcce695df13169bd885337e6074b923ab6edcfc8"},
+    {url = "https://files.pythonhosted.org/packages/da/f3/bc1581d8800bd5f82821bf3542b339fe44a75ddf669d36ff43a05f76322e/murmurhash-1.0.9-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:697ed01454d92681c7ae26eb1adcdc654b54062bcc59db38ed03cad71b23d449"},
+    {url = "https://files.pythonhosted.org/packages/e4/77/a48efb385f5ebc898f5f62e146ebad8e68745e3f5781fe263b4eaf8a8f8c/murmurhash-1.0.9-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:c0f84ecdf37c06eda0222f2f9e81c0974e1a7659c35b755ab2fdc642ebd366db"},
+    {url = "https://files.pythonhosted.org/packages/f6/24/30e74dc5970f357a897b3ec0fd44e1330c3f5fabefcfa0bc54c80b7ee0a5/murmurhash-1.0.9.tar.gz", hash = "sha256:fe7a38cb0d3d87c14ec9dddc4932ffe2dbc77d75469ab80fd5014689b0e07b58"},
+    {url = "https://files.pythonhosted.org/packages/fa/f0/71f0111f29e8a1f3487af3d0ffc846ab05637a0cfb67db514bc450039179/murmurhash-1.0.9-cp36-cp36m-win_amd64.whl", hash = "sha256:3e802fa5b0e618ee99e8c114ce99fc91677f14e9de6e18b945d91323a93c84e8"},
+    {url = "https://files.pythonhosted.org/packages/fb/d2/872e26de92082259f066dae0ea4d695c23125365802f8983a3e8f817ab53/murmurhash-1.0.9-cp37-cp37m-win_amd64.whl", hash = "sha256:8c3d69fb649c77c74a55624ebf7a0df3c81629e6ea6e80048134f015da57b2ea"},
+]
 "mutagen 1.46.0" = [
     {url = "https://files.pythonhosted.org/packages/03/ee/114d7016d2e34f341e212fefb5e7bd87785077ebcfff0ad23a497c70eea1/mutagen-1.46.0-py3-none-any.whl", hash = "sha256:8af0728aa2d5c3ee5a727e28d0627966641fddfe804c23eabb5926a4d770aed5"},
     {url = "https://files.pythonhosted.org/packages/b1/54/d1760a363d0fe345528e37782f6c18123b0e99e8ea755022fd51f1ecd0f9/mutagen-1.46.0.tar.gz", hash = "sha256:6e5f8ba84836b99fe60be5fb27f84be4ad919bbb6b49caa6ae81e70584b55e58"},
 ]
 "mypy-extensions 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/2a/e2/5d3f6ada4297caebe1a2add3b126fe800c96f56dbe5d1988a2cbe0b267aa/mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {url = "https://files.pythonhosted.org/packages/98/a4/1ab47638b92648243faf97a5aeb6ea83059cc3624972ab6b8d2316078d3f/mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
@@ -2058,61 +2344,61 @@
     {url = "https://files.pythonhosted.org/packages/f0/e8/1ea9adebdccaadfc208c7517e09f5145ed5a73069779ff436393085d47a2/numpy-1.24.3-cp311-cp311-win_amd64.whl", hash = "sha256:5342cf6aad47943286afa6f1609cad9b4266a05e7f2ec408e2cf7aea7ff69d80"},
     {url = "https://files.pythonhosted.org/packages/f3/23/7cc851bae09cf4db90d42a701dfe525780883ada86bece45e3da7a07e76b/numpy-1.24.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:3c1104d3c036fb81ab923f507536daedc718d0ad5a8707c6061cdfd6d184e570"},
     {url = "https://files.pythonhosted.org/packages/fa/7d/8dfb40eecbb6bc83ca00ef979f5cdeca5909a250cb8b642dcf1fbd34c078/numpy-1.24.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7"},
 ]
 "olefile 0.46" = [
     {url = "https://files.pythonhosted.org/packages/34/81/e1ac43c6b45b4c5f8d9352396a14144bba52c8fec72a80f425f6a4d653ad/olefile-0.46.zip", hash = "sha256:133b031eaf8fd2c9399b78b8bc5b8fcbe4c31e85295749bb17a87cba8f3c3964"},
 ]
-"orjson 3.8.12" = [
-    {url = "https://files.pythonhosted.org/packages/01/af/f0f1583194cb2b4e28b11e9c423d336e10ffee09939d86fa54ade60fe3ff/orjson-3.8.12-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:efb3a10030462a22c731682434df5c137a67632a8339f821cd501920b169007e"},
-    {url = "https://files.pythonhosted.org/packages/10/72/3e0c81df350632898725ca542538e648e28f6268542eff3fe0129290916c/orjson-3.8.12-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:6d1acf52d3a4b9384af09a5c2658c3a7a472a4d62a0ad1fe2c8fab8ef460c9b4"},
-    {url = "https://files.pythonhosted.org/packages/14/b7/18c54b14bdf6b1a805b706adfae2cc1a460de344ae1f6f8d5e1419093afe/orjson-3.8.12-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a72b50719bdd6bb0acfca3d4d1c841aa4b191f3ff37268e7aba04e5d6be44ccd"},
-    {url = "https://files.pythonhosted.org/packages/15/87/cd5a506935f80a75b0675aa06106efefb1379c1ed9bbb942794073cd8793/orjson-3.8.12-cp311-cp311-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:9a6c1594d5a9ff56e5babc4a87ac372af38d37adef9e06744e9f158431e33f43"},
-    {url = "https://files.pythonhosted.org/packages/16/f2/459afafc84fe178e30f593468d65a687449a49253ef217be151f398a0e0f/orjson-3.8.12-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:77710774faed337ac4ad919dadc5f3b655b0cd40518e5386e6f1f116de9c6c25"},
-    {url = "https://files.pythonhosted.org/packages/17/29/369a64bf87e66886e66962a1dd859b420bd79fec6771efffad94d56bd296/orjson-3.8.12-cp38-cp38-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:062e67108c218fdb9475edd5272b1629c05b56c66416fa915de5656adde30e73"},
-    {url = "https://files.pythonhosted.org/packages/17/68/bb2b4056589896f7500ac536331c713181bda9d29af8649bbdb359a5bc03/orjson-3.8.12-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:96fb1eb82b578eb6c0e53e3cf950839fe98ea210626f87c8204bd4fc2cc6ba02"},
-    {url = "https://files.pythonhosted.org/packages/18/22/440bd56050eb12ec7e4adf87386836385582d3801dcd4a6b00564d553559/orjson-3.8.12-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:4fd240e736ce52cd757d74142d9933fd35a3184396be887c435f0574e0388654"},
-    {url = "https://files.pythonhosted.org/packages/1a/ad/023133cbd08249a040fb4c422f8f527d557c9984eab83b2b5c9558c258b6/orjson-3.8.12-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6f568205519bb0197ca91915c5da6058cfbb59993e557b02dfc3b2718b34770a"},
-    {url = "https://files.pythonhosted.org/packages/26/2b/8f00f06ea857f00c3521e6a3fadf7e838a01faec7591cdbf217b25ad955d/orjson-3.8.12-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:becbd5af6d035a7ec2ee3239d4700929d52d8517806b97dd04efcc37289403f7"},
-    {url = "https://files.pythonhosted.org/packages/29/07/593edef4aefa554a7fb83d8616bffb76de0b6188b963dc74f75065668654/orjson-3.8.12-cp39-none-win_amd64.whl", hash = "sha256:82d65e478a21f98107b4eb8390104746bb3024c27084b57edab7d427385f1f70"},
-    {url = "https://files.pythonhosted.org/packages/29/9f/91d73b05f1bca62b815425e655e2b6d7da85f7f152955ca86a14af1c4db8/orjson-3.8.12-cp39-cp39-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:aff761de5ed5543a0a51e9f703668624749aa2239de5d7d37d9c9693daeaf5dc"},
-    {url = "https://files.pythonhosted.org/packages/2d/47/78b9f77454e5ba2adf527da5a4acb98e6d6291e162c0345649fe7f28b551/orjson-3.8.12-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:2ad149ed76dce2bbdfbadd61c35959305e77141badf364a158beb4ef3d88ec37"},
-    {url = "https://files.pythonhosted.org/packages/32/2f/6bd7d4e90dfe7d21a410907caceb9192c6595b1f8e3fca2a13c86e35cb34/orjson-3.8.12-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:62f999798f2fa55e567d483864ebfc30120fb055c2696a255979439323a5b15c"},
-    {url = "https://files.pythonhosted.org/packages/33/a5/a90f88d7e5c2d4281ee0a0fbf78dff31d1da8762787610924392200913ec/orjson-3.8.12-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:ebb03e4c7648f7bb299872002a6120082da018f41ba7a9ebf4ceae8d765443d2"},
-    {url = "https://files.pythonhosted.org/packages/35/f0/07ee02d463bc8964e723cdac48a6d928dcc021778b2eacd338339f6e67e1/orjson-3.8.12-cp37-none-win_amd64.whl", hash = "sha256:6f1b01f641f5e87168b819ac1cbd81aa6278e7572c326f3d27e92dea442a2c0d"},
-    {url = "https://files.pythonhosted.org/packages/3e/1d/e5628cd5828a325db7c1b3c241c99b76b1640ec2fd7b6eb6bd9895879e6b/orjson-3.8.12.tar.gz", hash = "sha256:9f0f042cf002a474a6aea006dd9f8d7a5497e35e5fb190ec78eb4d232ec19955"},
-    {url = "https://files.pythonhosted.org/packages/48/51/e1efdcaa98fd77527d3e46c9081d113c866af7f60317bdfc305c82e9fbca/orjson-3.8.12-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8682f752c19f6a7d9fc727fd98588b4c8b0dce791b5794bb814c7379ccd64a79"},
-    {url = "https://files.pythonhosted.org/packages/4f/fd/b8b27f9dce9e6b72968c5c955ca738c5a7cd3c0e98c48223151f587ea85f/orjson-3.8.12-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0ba645c92801417933fa74448622ba614a275ea82df05e888095c7742d913bb4"},
-    {url = "https://files.pythonhosted.org/packages/5a/98/98954742d267ed528c9a7a7317a165cdfd47c46cf32e71233925da1486b6/orjson-3.8.12-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:135f29cf936283a0cd1b8bce86540ca181108f2a4d4483eedad6b8026865d2a9"},
-    {url = "https://files.pythonhosted.org/packages/69/25/ed824928caac9ce7e609f023c8084fc61f4f21d106adaa724e0789a49836/orjson-3.8.12-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:44f7bb4c995652106276442de1147c9993716d1e2d79b7fd435afa154ff236b9"},
-    {url = "https://files.pythonhosted.org/packages/6b/df/bfba654be34cda184e7345606471f6f5320034d783bd0c9444e2be6858c7/orjson-3.8.12-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:834b50df79f1fe89bbaced3a1c1d8c8c92cc99e84cdcd374d8da4974b3560d2a"},
-    {url = "https://files.pythonhosted.org/packages/6e/ff/a2bd5781213b9770e7bb3beb1995ca1a4681d7a35bd00e6d1c65b5437063/orjson-3.8.12-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:355055e0977c43b0e5325b9312b7208c696fe20cd54eed1d6fc80b0a4d6721f5"},
-    {url = "https://files.pythonhosted.org/packages/70/54/2f31265e4021872397dec7d7d0b2baed6d59c7aa4910df73fae5fb6fdfcb/orjson-3.8.12-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c6390ce0bce24c107fc275736aa8a4f768ef7eb5df935d7dca0cc99815eb5d99"},
-    {url = "https://files.pythonhosted.org/packages/79/1e/50cf4ba0dc3a90233a0d4c75eae8fe7eb344a7f0638f61463a2cac13265f/orjson-3.8.12-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6cae2ff288a80e81ce30313e735c5436495ab58cf8d4fbe84900e616d0ee7a78"},
-    {url = "https://files.pythonhosted.org/packages/7b/fa/5011e7e3945147a61b2f5a798f6e5570fff5d7324bb8fa6a5a150dafdcd1/orjson-3.8.12-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:de3d096dde3e46d01841abc1982b906694ab3c92f338d37a2e6184739dc8a958"},
-    {url = "https://files.pythonhosted.org/packages/81/cb/5fe6078cd7425ddcbbf48aa5001bbf4cf7bfcd83992af4ded037b401b1b4/orjson-3.8.12-cp37-cp37m-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:7e549468867991f6f9cfbd9c5bbc977330173bd8f6ceb79973bbd4634e13e1b9"},
-    {url = "https://files.pythonhosted.org/packages/a5/63/a28607d7a7142a4e70d5571a2d3252de660f4cfc6b5e6e03efc608e3f4e6/orjson-3.8.12-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:397670665f94cf5cff779054781d80395084ba97191d82f7b3a86f0a20e6102b"},
-    {url = "https://files.pythonhosted.org/packages/a5/d3/cb28e1fccaa0740ed0f8562153651caabcd44589b6ee6960a0bf4f5e327d/orjson-3.8.12-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:d937503e4dfba5edc8d5e0426d3cc97ed55716e93212b2e12a198664487b9965"},
-    {url = "https://files.pythonhosted.org/packages/b0/e6/3242d5681358f65ead018d834d0e01f55c49347b06ba132931da49947a8e/orjson-3.8.12-cp310-none-win_amd64.whl", hash = "sha256:06e528f9a84fbb4000fd0eee573b5db543ee70ae586fdbc53e740b0ac981701c"},
-    {url = "https://files.pythonhosted.org/packages/b7/27/545b49651dca71eb92134935c49942c7be43672659c8db1b23d78c8d5a6d/orjson-3.8.12-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8d153b228b6e24f8bccf732a51e01e8e938eef59efed9030c5c257778fbe0804"},
-    {url = "https://files.pythonhosted.org/packages/bc/fe/b623cfe25ca9bdc3cb6cbefc6871ce3785363bfd38a30102dda44fbf4671/orjson-3.8.12-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:7e405d54c84c30d9b1c918c290bcf4ef484a45c69d5583a95db81ffffba40b44"},
-    {url = "https://files.pythonhosted.org/packages/bd/99/cfd8ef1b184ab9973517d450256d4f3a5b07ee958b0482819441c46cd7c3/orjson-3.8.12-cp37-cp37m-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:dc27a8ec13f28e92dc1ea89bf1232d77e7d3ebfd5c1ccf4f3729a70561cb63bd"},
-    {url = "https://files.pythonhosted.org/packages/bd/9d/6361f9333d9ec3593164e0cee538f66c1cdba317ff5f2d6e7debd5501541/orjson-3.8.12-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f480ae7b84369b1860d8867f0baf8d885fede400fda390ce088bfa8edf97ffdc"},
-    {url = "https://files.pythonhosted.org/packages/c5/76/1be359006bb9369ce52119ca6d0c30a408ecfb8726bdc61b7f444b53a046/orjson-3.8.12-cp38-none-win_amd64.whl", hash = "sha256:710c40c214b753392e46f9275fd795e9630dd737a5ab4ac6e4ee1a02fe83cc0d"},
-    {url = "https://files.pythonhosted.org/packages/c9/9e/1de9209a233ebaa6a013473bf17af25f1bd4b66653540dcf2f5618f633d0/orjson-3.8.12-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:f4e22b0aa70c963ac01fcd620de15be21a5027711b0e5d4b96debcdeea43e3ae"},
-    {url = "https://files.pythonhosted.org/packages/cc/08/a921138667cc064cee508e74a4c2e99afead8961552b047f3cbceb6dafaf/orjson-3.8.12-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:7d50d9b1ae409ea15534365fec0ce8a5a5f7dc94aa790aacfb8cfec87ab51aa4"},
-    {url = "https://files.pythonhosted.org/packages/cd/5e/f388c8f606c5c2aa047f93759ab94b1ff739cc99a9b95e507ca4bd242171/orjson-3.8.12-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:7d63f524048825e05950db3b6998c756d5377a5e8c469b2e3bdb9f3217523d74"},
-    {url = "https://files.pythonhosted.org/packages/cf/78/8f74d1670446455420c270792da794a8bc11bffc1f13fb2fa6803bd46837/orjson-3.8.12-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:8f00038bf5d07439d13c0c2c5cd6ad48eb86df7dbd7a484013ce6a113c421b14"},
-    {url = "https://files.pythonhosted.org/packages/d4/58/33619aab5d51f1948ab21aa7b26698a76ec9b1f2b5fb2af96dc3fd9a6833/orjson-3.8.12-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:cd6fbd1413559572e81b5ac64c45388147c3ba85cc3df2eaa11002945e0dbd1f"},
-    {url = "https://files.pythonhosted.org/packages/d6/18/e39890cbc4d2a6c4d7bc2202b960c3a6035df8f26b261d72da7b580f35ee/orjson-3.8.12-cp311-none-win_amd64.whl", hash = "sha256:eb16e0195febd24b44f4db1ab3be85ecf6038f92fd511370cebc004b3d422294"},
-    {url = "https://files.pythonhosted.org/packages/d7/b0/9ccdd107dc875e603edf9fa024680a2d63ab3e23464a4e78d5d1b8ecdde4/orjson-3.8.12-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:83e8c740a718fa6d511a82e463adc7ab17631c6eea81a716b723e127a9c51d57"},
-    {url = "https://files.pythonhosted.org/packages/d8/11/a9598459031b6601186352ad1441ae17ba8963b9dc7f7806b40dcedeff02/orjson-3.8.12-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:ec4f0130d9a27cb400423e09e0f9e46480e9e977f05fdcf663a7a2c68735513e"},
-    {url = "https://files.pythonhosted.org/packages/df/a1/5ec3a96568c40aa2ecf0220872691ef271454cadec1a6b761ae52f67bcbf/orjson-3.8.12-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3fa58ca064c640fa9d823f98fbbc8e71940ecb78cea3ac2507da1cbf49d60b51"},
-    {url = "https://files.pythonhosted.org/packages/e6/a7/d716cf8836515a85c349ad7fb1279536b7d59a1187b596a69cee66708e75/orjson-3.8.12-cp310-cp310-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:c84046e890e13a119404a83f2e09e622509ed4692846ff94c4ca03654fbc7fb5"},
-    {url = "https://files.pythonhosted.org/packages/f8/28/a1be6e66721ee95cff620a305447520e4c360bd8b9c9c7ba64c725262873/orjson-3.8.12-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:29706dd8189835bcf1781faed286e99ae54fd6165437d364dfdbf0276bf39b19"},
+"orjson 3.8.14" = [
+    {url = "https://files.pythonhosted.org/packages/03/bb/28d2ced376eebb93869eda6dbd7205597eb757220e39746bc088096b75f4/orjson-3.8.14-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:19415aaf30525a5baff0d72a089fcdd68f19a3674998263c885c3908228c1086"},
+    {url = "https://files.pythonhosted.org/packages/09/c6/4ba2bfc85dea2126a15b48933aa4e5dfaeaeac558808a83555c0c1af7831/orjson-3.8.14-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:e53bc5beb612df8ddddb065f079d3fd30b5b4e73053518524423549d61177f3f"},
+    {url = "https://files.pythonhosted.org/packages/10/32/c29c34bc0661277ea5493cfbe56a88746d5112c93db8990d25526f30b5e0/orjson-3.8.14-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:739f9f633e1544f2a477fa3bef380f488c8dca6e2521c8dc36424b12554ee31e"},
+    {url = "https://files.pythonhosted.org/packages/16/53/a961ea06b24422226df1e27158a5110b82cc8fa403a774a10323ce959e6d/orjson-3.8.14-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:04c70dc8ca79b0072a16d82f94b9d9dd6598a43dd753ab20039e9f7d2b14f017"},
+    {url = "https://files.pythonhosted.org/packages/1a/b7/983036df5ac56bbaaa91f34dbd2d0940998fbd259643cdd1c68b8db5714a/orjson-3.8.14-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:5fb66f0ac23e861b817c858515ac1f74d1cd9e72e3f82a5b2c9bae9f92286adc"},
+    {url = "https://files.pythonhosted.org/packages/1d/e5/2e39fe3ac903c0007984ac3a410b948e2c548853c6143510e06f4a8f56a8/orjson-3.8.14-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:27967be4c16bd09f4aeff8896d9be9cbd00fd72f5815d5980e4776f821e2f77c"},
+    {url = "https://files.pythonhosted.org/packages/21/17/3c75f22a4d8f120b13b23c46702a636e33bf6faefaca4833dd675d4df7c7/orjson-3.8.14-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:087c0dc93379e8ba2d59e9f586fab8de8c137d164fccf8afd5523a2137570917"},
+    {url = "https://files.pythonhosted.org/packages/25/44/1577b80174487557f04adf61c065c54bc90d77d29c0df0b440f0f289eb34/orjson-3.8.14-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7cb35dd3ba062c1d984d57e6477768ed7b62ed9260f31362b2d69106f9c60ebd"},
+    {url = "https://files.pythonhosted.org/packages/2a/60/f889bc75c6a8fc39f96499a71f8e69d7aa2fdc97193a45e707273c4d560f/orjson-3.8.14-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:ebca14ae80814219ea3327e3dfa7ff618621ff335e45781fac26f5cd0b48f2b4"},
+    {url = "https://files.pythonhosted.org/packages/2d/cb/d54d87ae58c3a09038458f5ad5efe93b3ab2f3d956ac47156469181777ef/orjson-3.8.14-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:38ca39bae7fbc050332a374062d4cdec28095540fa8bb245eada467897a3a0bb"},
+    {url = "https://files.pythonhosted.org/packages/2f/3a/1e89459e59fbc81ca3d5ff3465c8c7c55670552c2e08b7e437b6f2a016a2/orjson-3.8.14-cp310-none-win_amd64.whl", hash = "sha256:0bf00c42333412a9338297bf888d7428c99e281e20322070bde8c2314775508b"},
+    {url = "https://files.pythonhosted.org/packages/31/b4/9a11ba173208354fe2f393e8b2ea8e7dcd41ec3e8d044eb4ba7a1e9e3b61/orjson-3.8.14-cp37-cp37m-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:de1ee13d6b6727ee1db38722695250984bae81b8fc9d05f1176c74d14b1322d9"},
+    {url = "https://files.pythonhosted.org/packages/38/f5/85fd06d179e9c2cf6d9b46fd19e0d22463167c8623ce2100edf7dd5c3e36/orjson-3.8.14-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:67a7e883b6f782b106683979ccc43d89b98c28a1f4a33fe3a22e253577499bb1"},
+    {url = "https://files.pythonhosted.org/packages/3a/bb/425f0d9d0373fe82bc839009e4fa6e560e6dd9b2bbb67bfa02fb3c44caff/orjson-3.8.14-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:33bc310da4ad2ffe8f7f1c9e89692146d9ec5aec2d1c9ef6b67f8dc5e2d63241"},
+    {url = "https://files.pythonhosted.org/packages/43/de/5cdf2a1a218468190685f9a9490f566cd9f6b1101d03ceeddeb7f5cde3e7/orjson-3.8.14-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:9df820e6c8c84c52ec39ea2cc9c79f7999c839c7d1481a056908dce3b90ce9f9"},
+    {url = "https://files.pythonhosted.org/packages/4d/1c/e94425b29eaf3a34b58311d79ed2f2cc11caa7c838a60f59f9ecc5266625/orjson-3.8.14-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:aedba48264fe87e5060c0e9c2b28909f1e60626e46dc2f77e0c8c16939e2e1f7"},
+    {url = "https://files.pythonhosted.org/packages/4f/33/677d6ecec94e3ae639e0c5558dac64ea8b7fc08e48b986564773e6ea1245/orjson-3.8.14-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:062829b5e20cd8648bf4c11c3a5ee7cf196fa138e573407b5312c849b0cf354d"},
+    {url = "https://files.pythonhosted.org/packages/4f/54/7761dccc1a177f2259d291022c17d364340a061f5cb6d4133baa613b9efd/orjson-3.8.14-cp38-cp38-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:9f5cf61b6db68f213c805c55bf0aab9b4cb75a4e9c7f5bfbd4deb3a0aef0ec53"},
+    {url = "https://files.pythonhosted.org/packages/52/55/9f2277b6dbdba514889433ef892ad6735b15e774c69dcb6afde444439734/orjson-3.8.14-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:01640ab79111dd97515cba9fab7c66cb3b0967b0892cc74756a801ff681a01b6"},
+    {url = "https://files.pythonhosted.org/packages/5d/5e/4d5b1ea3bfde7595afa7ca57a16835e3cabe04cc3d624062048562b59e8e/orjson-3.8.14-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3ee09bfbf1d54c127d3061f6721a1a11d2ce502b50597c3d0d2e1bd2d235b764"},
+    {url = "https://files.pythonhosted.org/packages/6c/9b/7a7c65b44da3e405463bba712aac1ae5de77eca1b78ecd9a11c5c9b8ce43/orjson-3.8.14-cp38-none-win_amd64.whl", hash = "sha256:d03f29b0369bb1ab55c8a67103eb3a9675daaf92f04388568034fe16be48fa5d"},
+    {url = "https://files.pythonhosted.org/packages/6c/a4/a616e36bec0ca0e55a26b72b1e735a64d6c0d5203eabdcde4cd3498e802b/orjson-3.8.14-cp311-cp311-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:d66966fd94719beb84e8ed84833bc59c3c005d3d2d0c42f11d7552d3267c6de7"},
+    {url = "https://files.pythonhosted.org/packages/6e/ca/c50071a746ef136b4c120f4ec60d19d146b55c73301ba85058b161c40c87/orjson-3.8.14-cp37-none-win_amd64.whl", hash = "sha256:87ba7882e146e24a7d8b4a7971c20212c2af75ead8096fc3d55330babb1015fb"},
+    {url = "https://files.pythonhosted.org/packages/74/69/38b4676e007ae513499ab6fbe7260d7bfd2ea668b06d4d6c64e39293455f/orjson-3.8.14-cp311-none-win_amd64.whl", hash = "sha256:20b7ffc7736000ea205f9143df322b03961f287b4057606291c62c842ff3c5b5"},
+    {url = "https://files.pythonhosted.org/packages/8f/38/3d5630a9fa808d15f8c76de2a6318c45f3ad12c5dc3680572c6b3bd53e61/orjson-3.8.14-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:bf6825e160e4eb0ef65ce37d8c221edcab96ff2ffba65e5da2437a60a12b3ad1"},
+    {url = "https://files.pythonhosted.org/packages/90/20/73b99827beea76722b8b2a20b7b0b4003d267912b4f94f6933529d583e89/orjson-3.8.14-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:7e2f75b7d9285e35c3d4dff9811185535ff2ea637f06b2b242cb84385f8ffe63"},
+    {url = "https://files.pythonhosted.org/packages/94/7d/87bbb5e4d6368c6a7463ec60683cef924e6f60c1c167a8bada89d5e77137/orjson-3.8.14-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:92374bc35b6da344a927d5a850f7db80a91c7b837de2f0ea90fc870314b1ff44"},
+    {url = "https://files.pythonhosted.org/packages/9e/56/b2327648cc9e2e30f681c0121787cdbb1768c8c643666ebab1f268e2026c/orjson-3.8.14-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:ee0299b2dda9afce351a5e8c148ea7a886de213f955aa0288fb874fb44829c36"},
+    {url = "https://files.pythonhosted.org/packages/a0/2c/c8e38867801fb20ee4ffdc509550fad92e90e2c8c77d1d52e001e0d681e3/orjson-3.8.14-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6112194c11e611596eed72f46efb0e6b4812682eff3c7b48473d1146c3fa0efb"},
+    {url = "https://files.pythonhosted.org/packages/b2/ac/39719ba71753cc4a6ab67927809cdb7214aa83f10fabc91b957112ef1ed8/orjson-3.8.14-cp39-none-win_amd64.whl", hash = "sha256:9725226478d1dafe46d26f758eadecc6cf98dcbb985445e14a9c74aaed6ccfea"},
+    {url = "https://files.pythonhosted.org/packages/b5/96/f7dc7a640288b53e33ba772349066a6bbc8663e60a1d6bb64573709e93ae/orjson-3.8.14-cp37-cp37m-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:97ebb7fab5f1ae212a6501f17cb7750a6838ffc2f1cebbaa5dec1a90038ca3c6"},
+    {url = "https://files.pythonhosted.org/packages/bb/ed/4edbbb4af8d72ea678a030514f670ce53b289de8c46bd6cf2b72e8e0cce0/orjson-3.8.14-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:7d3d8faded5a514b80b56d0429eb38b429d7a810f8749d25dc10a0cc15b8a3c8"},
+    {url = "https://files.pythonhosted.org/packages/be/d1/bdc112671bd3c6373b8283889ba4d2bf34a7a029e33f58cf02b3d59abe30/orjson-3.8.14-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:0bc6b7abf27f1dc192dadad249df9b513912506dd420ce50fd18864a33789b71"},
+    {url = "https://files.pythonhosted.org/packages/c7/88/5c908d9ec55cad47d4a199535aac3f8aa2755fd85867f60ac1cc2c0c4bb5/orjson-3.8.14-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:31a2a29be559e92dcc5c278787b4166da6f0d45675b59a11c4867f5d1455ebf4"},
+    {url = "https://files.pythonhosted.org/packages/c8/a1/c7ded18ed1952bed15439f2331752b5ef0d33f1d9a0f9fdeee7549a84c8d/orjson-3.8.14.tar.gz", hash = "sha256:5ea93fd3ef7be7386f2516d728c877156de1559cda09453fc7dd7b696d0439b3"},
+    {url = "https://files.pythonhosted.org/packages/cd/1c/d6672a73e6359a4a767414246bad8216d44636809c9eea27e9a6938b3a7b/orjson-3.8.14-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8b206cca6836a4c6683bcaa523ab467627b5f03902e5e1082dc59cd010e6925f"},
+    {url = "https://files.pythonhosted.org/packages/cf/db/cdfed7a5efde531bdb7166db364ff4cf1f0b0c7e6edab0f9aecbbb855f08/orjson-3.8.14-cp39-cp39-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:716a3994e039203f0a59056efa28185d4cac51b922cc5bf27ab9182cfa20e12e"},
+    {url = "https://files.pythonhosted.org/packages/d1/d1/0ba3844cd12cbb01113a67a01ab3a77a9f59d7acaa346e517f2be6399def/orjson-3.8.14-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ca90db8f551b8960da95b0d4cad6c0489df52ea03585b6979595be7b31a3f946"},
+    {url = "https://files.pythonhosted.org/packages/d4/ad/d92c12caec047cb62ad56f169c29dcee6cbbec5de1abc863e71963cd14f6/orjson-3.8.14-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:09a3bf3154f40299b8bc95e9fb8da47436a59a2106fc22cae15f76d649e062da"},
+    {url = "https://files.pythonhosted.org/packages/d4/e5/5d8061ad5fc4907151e5c00db98d65f0590c9389672fefb93429b343dbe9/orjson-3.8.14-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:017de5ba22e58dfa6f41914f5edb8cd052d23f171000684c26b2d2ab219db31e"},
+    {url = "https://files.pythonhosted.org/packages/d9/47/4c30dca1f9b4b0d10c91381368554d8c7b89fc74889c8152f48ddcc84665/orjson-3.8.14-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:64b4fca0531030040e611c6037aaf05359e296877ab0a8e744c26ef9c32738b9"},
+    {url = "https://files.pythonhosted.org/packages/e3/ca/36ebce082fe66dd5f9555cc7ca2760ef593baaedd514aaf5eef0b7740303/orjson-3.8.14-cp310-cp310-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:7a7b0fead2d0115ef927fa46ad005d7a3988a77187500bf895af67b365c10d1f"},
+    {url = "https://files.pythonhosted.org/packages/e4/57/8331bd4ea3675ba72d96962346f0d9aabab7d2b11f00378adb42953ef004/orjson-3.8.14-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:8a896a12b38fe201a72593810abc1f4f1597e65b8c869d5fc83bbcf75d93398f"},
+    {url = "https://files.pythonhosted.org/packages/ea/f7/ca03a52cdda6d4702b554e446980f0278911abb2a0ebf7ec245bdf7ecc12/orjson-3.8.14-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:f80e62afe49e6bfc706e041faa351d7520b5f86572b8e31455802251ea989613"},
+    {url = "https://files.pythonhosted.org/packages/f4/18/a84b513905e1ed78529084967ca0b937f6ec45df200f908c4393aefddd79/orjson-3.8.14-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:f4ac01a3db4e6a98a8ad1bb1a3e8bfc777928939e87c04e93e0d5006df574a4b"},
+    {url = "https://files.pythonhosted.org/packages/f9/fa/35ba54c9ff8ba0c0759d8a496095f9fdf0ff7c18182c330784f6b3025754/orjson-3.8.14-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9393a63cb0424515ec5e434078b3198de6ec9e057f1d33bad268683935f0a5d5"},
 ]
 "packaging 23.1" = [
     {url = "https://files.pythonhosted.org/packages/ab/c3/57f0601a2d4fe15de7a553c00adbc901425661bf048f2a22dfc500caf121/packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {url = "https://files.pythonhosted.org/packages/b9/6c/7c6658d258d7971c5eb0d9b69fa9265879ec9a9158031206d47800ae2213/packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 "pandas 2.0.1" = [
     {url = "https://files.pythonhosted.org/packages/16/75/924e3a52c35cb105a152d29622d0f06bb0f48a677e77ddd6e11ef0004164/pandas-2.0.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e09a53a4fe8d6ae2149959a2d02e1ef2f4d2ceb285ac48f74b79798507e468b4"},
@@ -2145,14 +2431,18 @@
     {url = "https://files.pythonhosted.org/packages/05/63/8011bd08a4111858f79d2b09aad86638490d62fbf881c44e434a6dfca87b/parso-0.8.3-py2.py3-none-any.whl", hash = "sha256:c001d4636cd3aecdaf33cbb40aebb59b094be2a74c556778ef5576c175e19e75"},
     {url = "https://files.pythonhosted.org/packages/a2/0e/41f0cca4b85a6ea74d66d2226a7cda8e41206a624f5b330b958ef48e2e52/parso-0.8.3.tar.gz", hash = "sha256:8c07be290bb59f03588915921e29e8a50002acaf2cdc5fa0e0114f91709fafa0"},
 ]
 "pathspec 0.11.1" = [
     {url = "https://files.pythonhosted.org/packages/95/60/d93628975242cc515ab2b8f5b2fc831d8be2eff32f5a1be4776d49305d13/pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
     {url = "https://files.pythonhosted.org/packages/be/c8/551a803a6ebb174ec1c124e68b449b98a0961f0b737def601e3c1fbb4cfd/pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
 ]
+"pathy 0.10.1" = [
+    {url = "https://files.pythonhosted.org/packages/82/c6/683e3955de9a13b14dfa3ea358cd58f3914057e8064a2dcbfd450958e72e/pathy-0.10.1-py3-none-any.whl", hash = "sha256:a7613ee2d99a0a3300e1d836322e2d947c85449fde59f52906f995dbff67dad4"},
+    {url = "https://files.pythonhosted.org/packages/e9/fe/9fdf2ced8f3a4c25f3aac5141aad474b7701d288651472c9154a50b5a571/pathy-0.10.1.tar.gz", hash = "sha256:4cd6e71b4cd5ff875cfbb949ad9fa5519d8d1dbe69d5fc1d1b23aa3cb049618b"},
+]
 "pbr 5.11.1" = [
     {url = "https://files.pythonhosted.org/packages/01/06/4ab11bf70db5a60689fc521b636849c8593eb67a2c6bdf73a16c72d16a12/pbr-5.11.1-py2.py3-none-any.whl", hash = "sha256:567f09558bae2b3ab53cb3c1e2e33e726ff3338e7bae3db5dc954b3a44eef12b"},
     {url = "https://files.pythonhosted.org/packages/02/d8/acee75603f31e27c51134a858e0dea28d321770c5eedb9d1d673eb7d3817/pbr-5.11.1.tar.gz", hash = "sha256:aefc51675b0b533d56bb5fd1c8c6c0522fe31896679882e1c4c63d5e4a0fccb3"},
 ]
 "pdfminer-six 20191110" = [
     {url = "https://files.pythonhosted.org/packages/cb/83/200b2723bcbf1d1248a8a7d16e6dd6cb970b5331397b11948428d7ebcf37/pdfminer.six-20191110-py2.py3-none-any.whl", hash = "sha256:ca2ca58f3ac66a486bce53a6ddba95dc2b27781612915fa41c444790ba9cd2a8"},
     {url = "https://files.pythonhosted.org/packages/e8/31/7acc148333749d6a8ef7cbf25902bdf59a462811a69d040a9a259916b6bd/pdfminer.six-20191110.tar.gz", hash = "sha256:141a53ec491bee6d45bf9b2c7f82601426fb5d32636bcf6b9c8a8f3b6431fea6"},
@@ -2245,32 +2535,62 @@
     {url = "https://files.pythonhosted.org/packages/b3/93/55ae62910b94b46ecdd0ee8765289304f8df8deeaa1df7a96b0831c637ff/praw-7.7.0-py3-none-any.whl", hash = "sha256:22155c4b3006733a5ab0754136cf2226917747b61ec037ee335246fe0db5420e"},
     {url = "https://files.pythonhosted.org/packages/e5/f2/b784acf53cbb554dd7dd024f9095e1c89e74b294bba2fa187930f22f44cf/praw-7.7.0.tar.gz", hash = "sha256:090d209b35f79dfa36082ed1cdaa0f9a753b9277a69cfe8f9f32fa1827411a5a"},
 ]
 "prawcore 2.3.0" = [
     {url = "https://files.pythonhosted.org/packages/d6/36/55cc2cab22aafbebd52ddac4ccb670b920b54eb6ddbdb8573c79ca870d8a/prawcore-2.3.0-py3-none-any.whl", hash = "sha256:48c17db447fa06a13ca3e722201f443031437708daa736c05a1df895fbcceff5"},
     {url = "https://files.pythonhosted.org/packages/ed/85/13e76be737f3159514cce609b29e95499ba6d2cfa0b88761bab318b5f63e/prawcore-2.3.0.tar.gz", hash = "sha256:daf1ccd4b7a80dc4e6567d48336d782e94a9a6dad83770fc2edf76dc9a84f56d"},
 ]
+"preshed 3.0.8" = [
+    {url = "https://files.pythonhosted.org/packages/0b/60/40d8d8045aa1e735666350b1ea9f6334e2d65e71b04b01920d7771b405ff/preshed-3.0.8-cp37-cp37m-win_amd64.whl", hash = "sha256:85e98a618fb36cdcc37501d8b9b8c1246651cc2f2db3a70702832523e0ae12f4"},
+    {url = "https://files.pythonhosted.org/packages/12/69/8649e74b3f66d62a12bc3403ac3e4093ed5ac22648c8744d889e9e786f2c/preshed-3.0.8-cp36-cp36m-win_amd64.whl", hash = "sha256:09cc9da2ac1b23010ce7d88a5e20f1033595e6dd80be14318e43b9409f4c7697"},
+    {url = "https://files.pythonhosted.org/packages/13/38/e10ae90ee3cef36487aaa058dd0db60fa25dd1d9de911790c9d4c1e76e45/preshed-3.0.8-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:53d3e2456a085425c66af7baba62d7eaa24aa5e460e1a9e02c401a2ed59abd7b"},
+    {url = "https://files.pythonhosted.org/packages/20/c4/9661d9fb67e0c73ff892707d60b20cd8e10937e1ff5b720eafdd7d242b05/preshed-3.0.8-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:25b5ef5e387a0e17ff41202a8c1816184ab6fb3c0d0b847bf8add0ed5941eb8d"},
+    {url = "https://files.pythonhosted.org/packages/4b/b8/2ca85b2fbdf4e5c1e81cfd45da3c51f7789f3541941540a9efeefe6ffae9/preshed-3.0.8-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6a49ce52856fbb3ef4f1cc744c53f5d7e1ca370b1939620ac2509a6d25e02a50"},
+    {url = "https://files.pythonhosted.org/packages/52/cd/796a2ed6c906249da9d97f09228d16809c0328571297f742e1a08ad9b65f/preshed-3.0.8-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:7f8837bf616335464f3713cbf562a3dcaad22c3ca9193f957018964ef871a68b"},
+    {url = "https://files.pythonhosted.org/packages/5b/09/eac97626751799c75205dccd59d7e0105b1adca4a4e44ab7ebb67c51704a/preshed-3.0.8-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:e19c8069f1a1450f835f23d47724530cf716d581fcafb398f534d044f806b8c2"},
+    {url = "https://files.pythonhosted.org/packages/69/8a/f941bc420d5a07850157df71de69a7f8af6c0b097b5775c04c86404f7618/preshed-3.0.8-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:67643e66691770dc3434b01671648f481e3455209ce953727ef2330b16790aaa"},
+    {url = "https://files.pythonhosted.org/packages/6a/a8/fb3059ff92ab83f137a536448dcf037fb33e903bd44e453f6438a4472364/preshed-3.0.8-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5942858170c4f53d9afc6352a86bbc72fc96cc4d8964b6415492114a5920d3ed"},
+    {url = "https://files.pythonhosted.org/packages/74/a6/7a57125dcacea307af18bfaacc83003c388599cfbdff12b4f77f62e1fd0e/preshed-3.0.8-cp38-cp38-win_amd64.whl", hash = "sha256:246e7c6890dc7fe9b10f0e31de3346b906e3862b6ef42fcbede37968f46a73bf"},
+    {url = "https://files.pythonhosted.org/packages/77/35/4960a3486b2e95eaca4e14f9d13de50899aa115c72602225ae3ad789a08c/preshed-3.0.8-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8e945fc814bdc29564a2ce137c237b3a9848aa1e76a1160369b6e0d328151fdd"},
+    {url = "https://files.pythonhosted.org/packages/81/d7/5506d27522cc2594e512b89c29433842a24301d4bc2737215f6142fdf9c2/preshed-3.0.8-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fd19d48440b152657966a52e627780c0ddbe9d907b8d7ee4598505e80a3c55c7"},
+    {url = "https://files.pythonhosted.org/packages/8a/bb/c0534de9a1723eb96deeef731b6f63f8446992aa051a68f44261c83ffcd6/preshed-3.0.8-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:0e1bb8701df7861af26a312225bdf7c4822ac06fcf75aeb60fe2b0a20e64c222"},
+    {url = "https://files.pythonhosted.org/packages/8b/ae/34d7655667a3c7fccd4f38ab979a9c97999f0d6f41a5c1b98c702cd99004/preshed-3.0.8-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5a6a7fcf7dd2e7711051b3f0432da9ec9c748954c989f49d2cd8eabf8c2d953e"},
+    {url = "https://files.pythonhosted.org/packages/8f/10/89474a93d54a150ae729ff1468a6da1bc86074171a70c5e2eae532046f24/preshed-3.0.8-cp39-cp39-win_amd64.whl", hash = "sha256:06793022a56782ef51d74f1399925a2ba958e50c5cfbc6fa5b25c4945e158a07"},
+    {url = "https://files.pythonhosted.org/packages/99/22/1c34c6e2f69be8956614d11b2b27f4dab745efc78bed7ba4d8f18a5f9163/preshed-3.0.8-cp310-cp310-win_amd64.whl", hash = "sha256:c8a2e2931eea7e500fbf8e014b69022f3fab2e35a70da882e2fc753e5e487ae3"},
+    {url = "https://files.pythonhosted.org/packages/9e/44/b151e70e71ff00f950a08b7ef86597a719b25558ddf62bd2b2ba66f526ec/preshed-3.0.8-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fdbc2957b36115a576c515ffe963919f19d2683f3c76c9304ae88ef59f6b5ca6"},
+    {url = "https://files.pythonhosted.org/packages/9f/2d/1d3c658b14484e04d36fd31ae54854776d719b6b9283986ada23c20657ad/preshed-3.0.8-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e0ad3d860b9ce88a74cf7414bb4b1c6fd833813e7b818e76f49272c4974b19ce"},
+    {url = "https://files.pythonhosted.org/packages/a3/80/a43552e634284790e271694b82a7694cc08a06134155bb7b1d15e40373ae/preshed-3.0.8-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:e9aef2b0b7687aecef48b1c6ff657d407ff24e75462877dcb888fa904c4a9c6d"},
+    {url = "https://files.pythonhosted.org/packages/aa/69/fd5ecd05538cfcfa38853fc771f0063baecabf5939130e606f97f64e21d5/preshed-3.0.8-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:135e2ac0db1a3948d6ec295598c7e182b52c394663f2fcfe36a97ae51186be21"},
+    {url = "https://files.pythonhosted.org/packages/b3/a0/9fca34afe2dd03ee1a2eb8d5c9186ea914de3ddee29866b2ed8c0fca579b/preshed-3.0.8-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f9a4833530fe53001c351974e0c8bb660211b8d0358e592af185fec1ae12b2d0"},
+    {url = "https://files.pythonhosted.org/packages/d1/f4/e3a93cecfad1da8e3fae03585715fc0666a6ce50ba70f85f74c142254852/preshed-3.0.8-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e1472ee231f323b4f4368b1b5f8f08481ed43af89697d45450c6ae4af46ac08a"},
+    {url = "https://files.pythonhosted.org/packages/ea/ae/015fb8b2f901d46989990b922ac90743345706b8db66a9497cea11875098/preshed-3.0.8-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:720593baf2c2e295f855192974799e486da5f50d4548db93c44f5726a43cefb9"},
+    {url = "https://files.pythonhosted.org/packages/ed/1a/6cb1bf3fa4cb82bfdab3a1010c4b8708682e79b87716234d94067d0d2ceb/preshed-3.0.8-cp311-cp311-win_amd64.whl", hash = "sha256:019d8fa4161035811fb2804d03214143298739e162d0ad24e087bd46c50970f5"},
+    {url = "https://files.pythonhosted.org/packages/ed/9b/ce9af6f4eb6137b9a3289f2cd94812693039fe6067da142a5bd3ac872bcb/preshed-3.0.8-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:854d58a8913ebf3b193b0dc8064155b034e8987de25f26838dfeca09151fda8a"},
+    {url = "https://files.pythonhosted.org/packages/f1/78/c28a568317088b9cef21f8516bed2f41210492ae569c5842ad80251631a0/preshed-3.0.8.tar.gz", hash = "sha256:6c74c70078809bfddda17be96483c41d06d717934b07cab7921011d81758b357"},
+    {url = "https://files.pythonhosted.org/packages/f7/67/68f6be9f4c59f60e41c7e688b991958874eeb6d4d6ca3c12b3f793d20140/preshed-3.0.8-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:ea4b6df8ef7af38e864235256793bc3056e9699d991afcf6256fa298858582fc"},
+    {url = "https://files.pythonhosted.org/packages/fe/21/25d3e2dff5e9c83cd13668131d2f145f18ae0992238881a6e55fb888d869/preshed-3.0.8-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:0ae25a010c9f551aa2247ee621457f679e07c57fc99d3fd44f84cb40b925f12c"},
+]
 "prompt-toolkit 3.0.38" = [
     {url = "https://files.pythonhosted.org/packages/4b/bb/75cdcd356f57d17b295aba121494c2333d26bfff1a837e6199b8b83c415a/prompt_toolkit-3.0.38.tar.gz", hash = "sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b"},
     {url = "https://files.pythonhosted.org/packages/87/3f/1f5a0ff475ae6481f4b0d45d4d911824d3218b94ee2a97a8cb84e5569836/prompt_toolkit-3.0.38-py3-none-any.whl", hash = "sha256:45ea77a2f7c60418850331366c81cf6b5b9cf4c7fd34616f733c5427e6abbb1f"},
 ]
-"protobuf 4.23.1" = [
-    {url = "https://files.pythonhosted.org/packages/12/40/d5333cf8adbd6bf77bf33aecd96d69545424aa0fd63b9ae30cf6c61efa47/protobuf-4.23.1-cp310-abi3-win_amd64.whl", hash = "sha256:32e78beda26d7a101fecf15d7a4a792278a0d26a31bc327ff05564a9d68ab8ee"},
-    {url = "https://files.pythonhosted.org/packages/24/e7/f193d7480b5f777c64515f81c3b8c074c1d7b283695397d4f965441c6bc8/protobuf-4.23.1-cp310-abi3-win32.whl", hash = "sha256:410bcc0a5b279f634d3e16082ce221dfef7c3392fac723500e2e64d1806dd2be"},
-    {url = "https://files.pythonhosted.org/packages/2f/b4/966ccfcac26d8f56cacf56e4c0878d367ea9f5597be0144774fbc464271e/protobuf-4.23.1-cp39-cp39-win_amd64.whl", hash = "sha256:ac50be82491369a9ec3710565777e4da87c6d2e20404e0abb1f3a8f10ffd20f0"},
-    {url = "https://files.pythonhosted.org/packages/40/b7/700f2a5fc5aa009903d816a040ababcc7e5874df2deacb168f3a718b0d73/protobuf-4.23.1-cp37-abi3-manylinux2014_aarch64.whl", hash = "sha256:346990f634272caac1f09efbcfbbacb23098b1f606d172534c6fa2d9758bb436"},
-    {url = "https://files.pythonhosted.org/packages/49/be/78eb56a8c035bb582dbd89ec48b0be4f67288ae872d55d7698b3cb8b5562/protobuf-4.23.1-cp37-abi3-macosx_10_9_universal2.whl", hash = "sha256:f9510cac91e764e86acd74e2b7f7bc5e6127a7f3fb646d7c8033cfb84fd1176a"},
-    {url = "https://files.pythonhosted.org/packages/56/65/d1e5919fe13d46e8dabefe32526745c3ef1f47d88b0e1d5593fdbc1e1dd3/protobuf-4.23.1-cp37-cp37m-win_amd64.whl", hash = "sha256:3b8905eafe4439076e1f58e9d1fa327025fd2777cf90f14083092ae47f77b0aa"},
-    {url = "https://files.pythonhosted.org/packages/59/81/cdf57f5e952f7ff0512b9b04ba46424bf4fde1553feb710e1f1d9330be34/protobuf-4.23.1-cp38-cp38-win32.whl", hash = "sha256:5b9cd6097e6acae48a68cb29b56bc79339be84eca65b486910bb1e7a30e2b7c1"},
-    {url = "https://files.pythonhosted.org/packages/61/33/876ca85424503ae048ec3b765d228494eb27f240600835b5be6c23d1d209/protobuf-4.23.1-cp38-cp38-win_amd64.whl", hash = "sha256:decf119d54e820f298ee6d89c72d6b289ea240c32c521f00433f9dc420595f38"},
-    {url = "https://files.pythonhosted.org/packages/73/8b/926449627e192b022f71d2c48b51dbdc1271271e0fa4b809cff2dffab339/protobuf-4.23.1-cp37-abi3-manylinux2014_x86_64.whl", hash = "sha256:3ce113b3f3362493bddc9069c2163a38f240a9ed685ff83e7bcb756b05e1deb0"},
-    {url = "https://files.pythonhosted.org/packages/c7/fc/4775e99b4bc52309ac30e1751f260b8b637482b0e6647b397a52c4adff77/protobuf-4.23.1-cp39-cp39-win32.whl", hash = "sha256:91fac0753c3c4951fbb98a93271c43cc7cf3b93cf67747b3e600bb1e5cc14d61"},
-    {url = "https://files.pythonhosted.org/packages/d1/2a/bf4c68e2ef7552bbd9f6a17937fd46ab4eaee6b7b5e4723a6e00b4270144/protobuf-4.23.1-py3-none-any.whl", hash = "sha256:65f0ac96ef67d7dd09b19a46aad81a851b6f85f89725577f16de38f2d68ad477"},
-    {url = "https://files.pythonhosted.org/packages/d8/6c/a2a6fe10cdc9bc81e03be56139d5bc70427054eb0b3864b31ff9a2a4849d/protobuf-4.23.1.tar.gz", hash = "sha256:95789b569418a3e32a53f43d7763be3d490a831e9c08042539462b6d972c2d7e"},
-    {url = "https://files.pythonhosted.org/packages/e4/78/665cb3b2165c29037cea06e9d4774713a6bf1844dec118af98a8c427c24c/protobuf-4.23.1-cp37-cp37m-win32.whl", hash = "sha256:2036a3a1e7fc27f973fa0a7888dce712393af644f4695385f117886abc792e39"},
+"protobuf 4.23.2" = [
+    {url = "https://files.pythonhosted.org/packages/01/2b/d8d9f18f013869fb0ef1e10bcbe2c7d922f9852594dc16c61fd39da21231/protobuf-4.23.2-cp39-cp39-win_amd64.whl", hash = "sha256:54a533b971288af3b9926e53850c7eb186886c0c84e61daa8444385a4720297f"},
+    {url = "https://files.pythonhosted.org/packages/0a/1d/c3dea2372f3c39fd44c612c88b418c08d2a08f95168a560be8f6ed4f59d7/protobuf-4.23.2-cp38-cp38-win32.whl", hash = "sha256:6c081863c379bb1741be8f8193e893511312b1d7329b4a75445d1ea9955be69e"},
+    {url = "https://files.pythonhosted.org/packages/14/23/f3b852093f3a7031049313913e04431e7a32bd9752adfaf79d1193cf05b1/protobuf-4.23.2-cp37-abi3-manylinux2014_x86_64.whl", hash = "sha256:86df87016d290143c7ce3be3ad52d055714ebaebb57cc659c387e76cfacd81aa"},
+    {url = "https://files.pythonhosted.org/packages/1d/af/4e351c0157d5a0440dc3ac0b3c1fdaa036b3b446bf98310b5e3d6d9d2733/protobuf-4.23.2-py3-none-any.whl", hash = "sha256:8da6070310d634c99c0db7df48f10da495cc283fd9e9234877f0cd182d43ab7f"},
+    {url = "https://files.pythonhosted.org/packages/5b/bc/d858096c9867968b184048a1c4048aa7fa95c69f3b7d10ea18d1061c7e65/protobuf-4.23.2-cp37-cp37m-win32.whl", hash = "sha256:281342ea5eb631c86697e1e048cb7e73b8a4e85f3299a128c116f05f5c668f8f"},
+    {url = "https://files.pythonhosted.org/packages/7f/2e/49d5a453d68febffbb602ad985b7432377e36bdf47198c6ab05021b33016/protobuf-4.23.2.tar.gz", hash = "sha256:20874e7ca4436f683b64ebdbee2129a5a2c301579a67d1a7dda2cdf62fb7f5f7"},
+    {url = "https://files.pythonhosted.org/packages/8b/e8/778843c7d969167a8be2967a19f55b50ee286fe44ceac17283beafc27fae/protobuf-4.23.2-cp37-abi3-macosx_10_9_universal2.whl", hash = "sha256:b2cfab63a230b39ae603834718db74ac11e52bccaaf19bf20f5cce1a84cf76df"},
+    {url = "https://files.pythonhosted.org/packages/b2/0b/5dad6967d12c4333c3389fb0648e32a143296b4c8e93dd6330da7cb51c71/protobuf-4.23.2-cp39-cp39-win32.whl", hash = "sha256:efabbbbac1ab519a514579ba9ec52f006c28ae19d97915951f69fa70da2c9e91"},
+    {url = "https://files.pythonhosted.org/packages/b4/39/be34246e573270e3db7bc74690ddfdaf5d5b267129d657d278949a496572/protobuf-4.23.2-cp37-abi3-manylinux2014_aarch64.whl", hash = "sha256:c52cfcbfba8eb791255edd675c1fe6056f723bf832fa67f0442218f8817c076e"},
+    {url = "https://files.pythonhosted.org/packages/b5/c6/8b23679288c7135d1be7972e7c1435ea21be8b380d8b88b5627f7dc58851/protobuf-4.23.2-cp310-abi3-win32.whl", hash = "sha256:384dd44cb4c43f2ccddd3645389a23ae61aeb8cfa15ca3a0f60e7c3ea09b28b3"},
+    {url = "https://files.pythonhosted.org/packages/be/13/dcec82bd1799f0be81217eb78eaa0db5d47c1b90acaee03417d2aa888a41/protobuf-4.23.2-cp37-cp37m-win_amd64.whl", hash = "sha256:ce744938406de1e64b91410f473736e815f28c3b71201302612a68bf01517fea"},
+    {url = "https://files.pythonhosted.org/packages/e7/ed/7472101221493605af740238fa72bd10c9965e05c50b3ef7904c7cad712c/protobuf-4.23.2-cp310-abi3-win_amd64.whl", hash = "sha256:09310bce43353b46d73ba7e3bca78273b9bc50349509b9698e64d288c6372c2a"},
+    {url = "https://files.pythonhosted.org/packages/f2/07/9f7717f8b8a1bfd00d50c367ff8cc1ad23bde1106f914e5e74c7fb18bd92/protobuf-4.23.2-cp38-cp38-win_amd64.whl", hash = "sha256:25e3370eda26469b58b602e29dff069cfaae8eaa0ef4550039cc5ef8dc004511"},
 ]
 "psutil 5.8.0" = [
     {url = "https://files.pythonhosted.org/packages/10/d6/c5c19e40bb05e2cb5f053f480dfe47e9543a8322f1a5985d7352bf689611/psutil-5.8.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:6223d07a1ae93f86451d0198a0c361032c4c93ebd4bf6d25e2fb3edfad9571ef"},
     {url = "https://files.pythonhosted.org/packages/12/80/8d09c345f19af2b29a309f8f9284e3ba1ae1ebd9438419080c14630f743a/psutil-5.8.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6323d5d845c2785efb20aded4726636546b26d3b577aded22492908f7c1bdda7"},
     {url = "https://files.pythonhosted.org/packages/15/28/47c28171fd7eeb83df74f78ccac090211f4a49408f376eb8e78a7bb47dc0/psutil-5.8.0-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:02b8292609b1f7fcb34173b25e48d0da8667bc85f81d7476584d889c6e0f2131"},
     {url = "https://files.pythonhosted.org/packages/18/c9/1db6aa0d28831f60408a6aab9d108c2edbd5a9ed11e5957a91d9d8023898/psutil-5.8.0-cp37-cp37m-win32.whl", hash = "sha256:1bff0d07e76114ec24ee32e7f7f8d0c4b0514b3fae93e3d2aaafd65d22502394"},
     {url = "https://files.pythonhosted.org/packages/19/29/f7a38ee30083f2caa14cc77a6d34c4d5cfd1a69641e87bf1b3d6ba90d0ba/psutil-5.8.0-cp36-cp36m-win32.whl", hash = "sha256:36b3b6c9e2a34b7d7fbae330a85bf72c30b1c827a4366a07443fc4b6270449e2"},
@@ -2310,83 +2630,119 @@
     {url = "https://files.pythonhosted.org/packages/b3/a7/7bd0c86e0c07872a391085c5896257807186c4436365547747cd75239e83/PyChromecast-13.0.7-py2.py3-none-any.whl", hash = "sha256:2327f1a2c3902e7be901f43dc97e65aeebb42f0d0a8b2c29f55453c6cacc3bd0"},
     {url = "https://files.pythonhosted.org/packages/d9/cb/d3e8dd7384e2bb4db859486b7a73355934288d65c6f45c65ae59f6abea25/PyChromecast-13.0.7.tar.gz", hash = "sha256:0de98e9e5be43269dd41efb16126ab0d5ba941ca4acae024329712851c0c0324"},
 ]
 "pycparser 2.21" = [
     {url = "https://files.pythonhosted.org/packages/5e/0b/95d387f5f4433cb0f53ff7ad859bd2c6051051cebbb564f139a999ab46de/pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
     {url = "https://files.pythonhosted.org/packages/62/d5/5f610ebe421e85889f2e55e33b7f9a6795bd982198517d912eb1c76e1a53/pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
 ]
-"pycryptodome 3.17" = [
-    {url = "https://files.pythonhosted.org/packages/05/6e/ffedda1885ccb5ab52911cfd38ee834c5fa1df1f500f0da34f92b52f70e1/pycryptodome-3.17-cp35-abi3-macosx_10_9_universal2.whl", hash = "sha256:e7debd9c439e7b84f53be3cf4ba8b75b3d0b6e6015212355d6daf44ac672e210"},
-    {url = "https://files.pythonhosted.org/packages/0a/ac/4e53706aa59841b0d0840862cb424a92057922638d58e5d03cc9fa56f2f0/pycryptodome-3.17-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:3a232474cd89d3f51e4295abe248a8b95d0332d153bf46444e415409070aae1e"},
-    {url = "https://files.pythonhosted.org/packages/14/58/77278d7a078241b55b515f6073b90108125fb0d197b384a0f372c5f61c80/pycryptodome-3.17-cp35-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:80ea8333b6a5f2d9e856ff2293dba2e3e661197f90bf0f4d5a82a0a6bc83a626"},
-    {url = "https://files.pythonhosted.org/packages/14/7a/f764564dceaf131e7a740c618d6bdfc30e2ca264e9de410ca757f6c4c3e3/pycryptodome-3.17-cp35-abi3-win_amd64.whl", hash = "sha256:9ec565e89a6b400eca814f28d78a9ef3f15aea1df74d95b28b7720739b28f37f"},
-    {url = "https://files.pythonhosted.org/packages/2b/1e/d928db092e1d445eb27b565c3a889922a33dd4bf8e5177b854024a88a7d9/pycryptodome-3.17-pp27-pypy_73-macosx_10_9_x86_64.whl", hash = "sha256:e1819b67bcf6ca48341e9b03c2e45b1c891fa8eb1a8458482d14c2805c9616f2"},
-    {url = "https://files.pythonhosted.org/packages/3d/7f/0cc8b6f606f2b5e728e196ad1e5781f5cc7eb0739cd9b801dbb971540384/pycryptodome-3.17-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:53068e33c74f3b93a8158dacaa5d0f82d254a81b1002e0cd342be89fcb3433eb"},
-    {url = "https://files.pythonhosted.org/packages/44/02/f28982e35dedde733ac2be8d890e42e752b39df8db0487dcc8923339ec06/pycryptodome-3.17-cp27-cp27m-win_amd64.whl", hash = "sha256:87e2ca3aa557781447428c4b6c8c937f10ff215202ab40ece5c13a82555c10d6"},
-    {url = "https://files.pythonhosted.org/packages/48/0d/0ec990bc94eab7dec1aeea19ba171973e9b206f3ef845f7822cd5f684e95/pycryptodome-3.17-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:38bbd6717eac084408b4094174c0805bdbaba1f57fc250fd0309ae5ec9ed7e09"},
-    {url = "https://files.pythonhosted.org/packages/4b/7e/652bae880c1e63efa0da60ed0c8709d82aa853557d51113098db217f3f0d/pycryptodome-3.17-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:04779cc588ad8f13c80a060b0b1c9d1c203d051d8a43879117fe6b8aaf1cd3fa"},
-    {url = "https://files.pythonhosted.org/packages/51/49/83d54682b9661f195fd9e78c83280451e1a73b396d988b359c1b8f6ae06a/pycryptodome-3.17-cp27-cp27mu-musllinux_1_1_aarch64.whl", hash = "sha256:5587803d5b66dfd99e7caa31ed91fba0fdee3661c5d93684028ad6653fce725f"},
-    {url = "https://files.pythonhosted.org/packages/52/54/70c63a8cf3280ad0ea317f4078333b02854170b78080e421c4b56294019e/pycryptodome-3.17-cp35-abi3-musllinux_1_1_i686.whl", hash = "sha256:1a30f51b990994491cec2d7d237924e5b6bd0d445da9337d77de384ad7f254f9"},
-    {url = "https://files.pythonhosted.org/packages/57/ed/2cfec0ee52cb1089cc1a4d0fb79492b2c84460a3fd2b6beaab8e77754a51/pycryptodome-3.17-cp35-abi3-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c133f6721fba313722a018392a91e3c69d3706ae723484841752559e71d69dc6"},
-    {url = "https://files.pythonhosted.org/packages/68/3f/58dcf1905579f0124aecb00860c0e7f829b0694baf1e2878ba5c079b6b30/pycryptodome-3.17-cp27-cp27m-win32.whl", hash = "sha256:ba2d4fcb844c6ba5df4bbfee9352ad5352c5ae939ac450e06cdceff653280450"},
-    {url = "https://files.pythonhosted.org/packages/6b/45/4d95ff046314f4185dd0a50204d0e9bed10663e837c41c4cce14e3b6be19/pycryptodome-3.17-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:f44c0d28716d950135ff21505f2c764498eda9d8806b7c78764165848aa419bc"},
-    {url = "https://files.pythonhosted.org/packages/72/86/d2e3f764fc0c646bbf6d6ca61ea51546c97cd98430a602501fa9ec0a40ca/pycryptodome-3.17-cp35-abi3-win32.whl", hash = "sha256:a3228728a3808bc9f18c1797ec1179a0efb5068c817b2ffcf6bcd012494dffb2"},
-    {url = "https://files.pythonhosted.org/packages/75/25/10831dec324a285cc54e476ce5982b9b81a60a49b67b1751ae879cd602d5/pycryptodome-3.17-cp27-cp27m-manylinux2014_aarch64.whl", hash = "sha256:9453b4e21e752df8737fdffac619e93c9f0ec55ead9a45df782055eb95ef37d9"},
-    {url = "https://files.pythonhosted.org/packages/83/3e/7ace48c22cd605464c296c49bc40fdaef83626fcbf15097ff9414f873377/pycryptodome-3.17-pp27-pypy_73-win32.whl", hash = "sha256:afbcdb0eda20a0e1d44e3a1ad6d4ec3c959210f4b48cabc0e387a282f4c7deb8"},
-    {url = "https://files.pythonhosted.org/packages/89/b3/37bc985bd473c25cd8fa1131a0da8401eac3753c1e035eecf8c9ae46638d/pycryptodome-3.17-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:5a790bc045003d89d42e3b9cb3cc938c8561a57a88aaa5691512e8540d1ae79c"},
-    {url = "https://files.pythonhosted.org/packages/8b/2a/0cfadd425e1fa848111d8faeb5b3e8e3aa1d76eaad94550302df5eab0ff6/pycryptodome-3.17-cp27-cp27mu-manylinux2014_aarch64.whl", hash = "sha256:d086d46774e27b280e4cece8ab3d87299cf0d39063f00f1e9290d096adc5662a"},
-    {url = "https://files.pythonhosted.org/packages/8e/bb/eeb7a1d70b53234fefdc338b5808fa7fe0063144d09087a1ed3baddc6e93/pycryptodome-3.17-cp27-cp27m-musllinux_1_1_aarch64.whl", hash = "sha256:121d61663267f73692e8bde5ec0d23c9146465a0d75cad75c34f75c752527b01"},
-    {url = "https://files.pythonhosted.org/packages/96/58/bf40ec413a6b88e378bfcf8e83a3c258c7b8cf0cb61e47100512c5ac56a7/pycryptodome-3.17-pp27-pypy_73-manylinux2010_x86_64.whl", hash = "sha256:f8e550caf52472ae9126953415e4fc554ab53049a5691c45b8816895c632e4d7"},
-    {url = "https://files.pythonhosted.org/packages/96/5e/c3c0591f1ff28787f302dd6459e059d8d503393ca3a7b0f150c48adac050/pycryptodome-3.17-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:8198f2b04c39d817b206ebe0db25a6653bb5f463c2319d6f6d9a80d012ac1e37"},
-    {url = "https://files.pythonhosted.org/packages/9d/98/93da5981fea934be5bd60d87e4bdee1e157b565b7b730e09766b478fd0ba/pycryptodome-3.17-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:74794a2e2896cd0cf56fdc9db61ef755fa812b4a4900fa46c49045663a92b8d0"},
-    {url = "https://files.pythonhosted.org/packages/b0/19/25bbc06ab3556803635a3ef2dc334eb5aa5d546083f26bc6d2d553ce2786/pycryptodome-3.17-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:2c5631204ebcc7ae33d11c43037b2dafe25e2ab9c1de6448eb6502ac69c19a56"},
-    {url = "https://files.pythonhosted.org/packages/b1/de/d167099339f8bc971da9b7258680020729c10a84678f2fc9f160eaf31fa7/pycryptodome-3.17-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f68d6c8ea2974a571cacb7014dbaada21063a0375318d88ac1f9300bc81e93c3"},
-    {url = "https://files.pythonhosted.org/packages/b5/9c/063b2a6c8eb5e9269b53e322e9cba56d299a6e67ba36ed8aa2af1be8b21b/pycryptodome-3.17-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:a74f45aee8c5cc4d533e585e0e596e9f78521e1543a302870a27b0ae2106381e"},
-    {url = "https://files.pythonhosted.org/packages/b8/2e/cf9cfd1ae6429381d3d9c14c8df79d91ae163929972f245a76058ea9d37d/pycryptodome-3.17.tar.gz", hash = "sha256:bce2e2d8e82fcf972005652371a3e8731956a0c1fbb719cc897943b3695ad91b"},
-    {url = "https://files.pythonhosted.org/packages/bc/14/c37136acac4aa4fa3980bdbae5d167b36b039775eeeef6cd61529840f2bf/pycryptodome-3.17-cp35-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:909e36a43fe4a8a3163e9c7fc103867825d14a2ecb852a63d3905250b308a4e5"},
-    {url = "https://files.pythonhosted.org/packages/d2/f4/55bafc39cd2b268398eba63f8846e5649923590977f3826e625a663998fa/pycryptodome-3.17-cp35-abi3-manylinux2014_aarch64.whl", hash = "sha256:dc22cc00f804485a3c2a7e2010d9f14a705555f67020eb083e833cabd5bd82e4"},
-    {url = "https://files.pythonhosted.org/packages/ea/7d/690febdf9d8831f13531b452e38258925e369246cbefbb1c325b0210f053/pycryptodome-3.17-cp35-abi3-macosx_10_9_x86_64.whl", hash = "sha256:ca1ceb6303be1282148f04ac21cebeebdb4152590842159877778f9cf1634f09"},
-    {url = "https://files.pythonhosted.org/packages/eb/e5/cf0c2809e18619d593504fd17a8c2284a76a269f57499226d7aaca360cfb/pycryptodome-3.17-cp35-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:333306eaea01fde50a73c4619e25631e56c4c61bd0fb0a2346479e67e3d3a820"},
-    {url = "https://files.pythonhosted.org/packages/ec/c1/22f08e3e29b9e63e366624129ad6b1cb0226a6bc1e136590dddefdec9986/pycryptodome-3.17-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4992ec965606054e8326e83db1c8654f0549cdb26fce1898dc1a20bc7684ec1c"},
-    {url = "https://files.pythonhosted.org/packages/f5/c6/81a181a8ef514ec3ecd8c498e13f8cec3a75caff2c501672d0e4993e1afc/pycryptodome-3.17-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:f812d58c5af06d939b2baccdda614a3ffd80531a26e5faca2c9f8b1770b2b7af"},
-]
-"pycryptodomex 3.17" = [
-    {url = "https://files.pythonhosted.org/packages/08/7c/4b55006bc7615db176a52feb7ec49201048045dd08ec38bbeae2d59e2456/pycryptodomex-3.17-cp35-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:78f0ddd4adc64baa39b416f3637aaf99f45acb0bcdc16706f0cc7ebfc6f10109"},
-    {url = "https://files.pythonhosted.org/packages/0c/7c/216750deab65e0e8a69b9b90d2bcdb18e9deabe30f4687773772010b0c9d/pycryptodomex-3.17-pp27-pypy_73-macosx_10_9_x86_64.whl", hash = "sha256:d4cf0128da167562c49b0e034f09e9cedd733997354f2314837c2fa461c87bb1"},
-    {url = "https://files.pythonhosted.org/packages/19/82/67d95bde8d1fbadd8239c895fa5873ec001bc3f731bec5fca29dc9c7dfa4/pycryptodomex-3.17-cp27-cp27m-win32.whl", hash = "sha256:a57e3257bacd719769110f1f70dd901c5b6955e9596ad403af11a3e6e7e3311c"},
-    {url = "https://files.pythonhosted.org/packages/21/49/bbde1ffbe18169916c8a26eb157ad97cab5f39d156d8e4b84afec8ac2feb/pycryptodomex-3.17-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:4c4674f4b040321055c596aac926d12f7f6859dfe98cd12f4d9453b43ab6adc8"},
-    {url = "https://files.pythonhosted.org/packages/2b/b0/e237622b6e2631d9eaa7aa237a9f321299b9fe49500d0f56851eb1c703a2/pycryptodomex-3.17-cp27-cp27mu-musllinux_1_1_aarch64.whl", hash = "sha256:7cc28dd33f1f3662d6da28ead4f9891035f63f49d30267d3b41194c8778997c8"},
-    {url = "https://files.pythonhosted.org/packages/2f/64/94bb7674fa02eac6564c0f5eab20d7d01cb60d4a457b17b14c7abbb8a367/pycryptodomex-3.17-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:3c2516b42437ae6c7a29ef3ddc73c8d4714e7b6df995b76be4695bbe4b3b5cd2"},
-    {url = "https://files.pythonhosted.org/packages/37/ba/0a71535124f781bb8ced7028dd2b36be3835a854030eb55e5d0eb809d20b/pycryptodomex-3.17-cp35-abi3-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a4fa037078e92c7cc49f6789a8bac3de06856740bb2038d05f2d9a2e4b165d59"},
-    {url = "https://files.pythonhosted.org/packages/3d/07/cfd8f52b9068877801317d26dc7225e19421bc659e1395d2cd6933b1a351/pycryptodomex-3.17.tar.gz", hash = "sha256:0af93aad8d62e810247beedef0261c148790c52f3cd33643791cc6396dd217c1"},
-    {url = "https://files.pythonhosted.org/packages/3e/f5/bbc11cd3655ad93563defcab7894bdb0e71c9e77d9b86edac747215dd28d/pycryptodomex-3.17-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:64b876d57cb894b31056ad8dd6a6ae1099b117ae07a3d39707221133490e5715"},
-    {url = "https://files.pythonhosted.org/packages/51/71/855ea0995a1e8afd79de2d762e2053d047b343ce50285c29ef19281908b4/pycryptodomex-3.17-cp35-abi3-manylinux2014_aarch64.whl", hash = "sha256:7fa0b52df90343fafe319257b31d909be1d2e8852277fb0376ba89d26d2921db"},
-    {url = "https://files.pythonhosted.org/packages/63/f4/34b68753be7a5e727bffb6a336ca75715572c58b9649d96af6ba9af364e9/pycryptodomex-3.17-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ee8bf4fdcad7d66beb744957db8717afc12d176e3fd9c5d106835133881a049b"},
-    {url = "https://files.pythonhosted.org/packages/65/0a/4759f7694cb4904d135041ba57371f1fdeb1e54086de205fd181d75f908a/pycryptodomex-3.17-cp27-cp27m-win_amd64.whl", hash = "sha256:d38ab9e53b1c09608ba2d9b8b888f1e75d6f66e2787e437adb1fecbffec6b112"},
-    {url = "https://files.pythonhosted.org/packages/67/1d/ee1a7f2553433b31fc70731a2fe72a26f28fedc7e7933715d16c8da6567d/pycryptodomex-3.17-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:67a3648025e4ddb72d43addab764336ba2e670c8377dba5dd752e42285440d31"},
-    {url = "https://files.pythonhosted.org/packages/72/7a/142990b5e9ce6032065decfd617cc9bd650539fc72711730b74228ff5217/pycryptodomex-3.17-cp35-abi3-musllinux_1_1_i686.whl", hash = "sha256:6feedf4b0e36b395329b4186a805f60f900129cdf0170e120ecabbfcb763995d"},
-    {url = "https://files.pythonhosted.org/packages/73/0a/6f78b1ec45ce22ed2e61185d52e55325f14f09ffcccfd938c0a20f9d7f0e/pycryptodomex-3.17-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:23d83b610bd97704f0cd3acc48d99b76a15c8c1540d8665c94d514a49905bad7"},
-    {url = "https://files.pythonhosted.org/packages/78/db/ec162a8fa1c7c8e03488616a01de59bb752b985f1c507ffb127b40b9d456/pycryptodomex-3.17-cp35-abi3-macosx_10_9_x86_64.whl", hash = "sha256:55eed98b4150a744920597c81b3965b632038781bab8a08a12ea1d004213c600"},
-    {url = "https://files.pythonhosted.org/packages/79/8b/6ae6f03e3b09b6e480507a488ea58a00eae44063fb8fce39e6cb01533237/pycryptodomex-3.17-pp27-pypy_73-win32.whl", hash = "sha256:599bb4ae4bbd614ca05f49bd4e672b7a250b80b13ae1238f05fd0f09d87ed80a"},
-    {url = "https://files.pythonhosted.org/packages/7d/6e/659b7cffab6914cb589ab8460eadd93b9670840c04d69490a506b6fd792c/pycryptodomex-3.17-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:5c23482860302d0d9883404eaaa54b0615eefa5274f70529703e2c43cc571827"},
-    {url = "https://files.pythonhosted.org/packages/7e/d5/34375b3646bc3387f8b5e8ff5e5d95a625b683c04ad89eb06ac1de9157fb/pycryptodomex-3.17-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:fd29d35ac80755e5c0a99d96b44fb9abbd7e871849581ea6a4cb826d24267537"},
-    {url = "https://files.pythonhosted.org/packages/7f/5f/d28db7498fa8047d8b7a1a2a47a5f48e1007d2030340eb44cbf19c29b35c/pycryptodomex-3.17-cp35-abi3-win32.whl", hash = "sha256:32e764322e902bbfac49ca1446604d2839381bbbdd5a57920c9daaf2e0b778df"},
-    {url = "https://files.pythonhosted.org/packages/80/6b/98b59492a545da19f8c892904f18c4386adb11ee93cd3ec10083b80be44d/pycryptodomex-3.17-pp27-pypy_73-manylinux2010_x86_64.whl", hash = "sha256:c92537b596bd5bffb82f8964cabb9fef1bca8a28a9e0a69ffd3ec92a4a7ad41b"},
-    {url = "https://files.pythonhosted.org/packages/86/aa/f7cfe88bc0de8fc64d7deb25e13fe200bc8ba8bda1a7a2f2c41d01b74505/pycryptodomex-3.17-cp35-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:7a6651a07f67c28b6e978d63aa3a3fccea0feefed9a8453af3f7421a758461b7"},
-    {url = "https://files.pythonhosted.org/packages/8b/74/731dc28961e5ec2da3a3fb504a934d125c2f69fa1433636754dddd4db22f/pycryptodomex-3.17-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:ab33c2d9f275e05e235dbca1063753b5346af4a5cac34a51fa0da0d4edfb21d7"},
-    {url = "https://files.pythonhosted.org/packages/95/0c/fe7dcd9942d3373ec91d0ca9eacb94f5e7204be2e08d92e98dfda01dbced/pycryptodomex-3.17-cp35-abi3-macosx_10_9_universal2.whl", hash = "sha256:2d4d395f109faba34067a08de36304e846c791808524614c731431ee048fe70a"},
-    {url = "https://files.pythonhosted.org/packages/99/54/07b44e8aec6cb303c9695561a6f50d4212e15989bdba7363517ada77f8b9/pycryptodomex-3.17-cp35-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:88b0d5bb87eaf2a31e8a759302b89cf30c97f2f8ca7d83b8c9208abe8acb447a"},
-    {url = "https://files.pythonhosted.org/packages/a4/ab/bde641549132cc3377ff75e0e5be7766a68e916a51817b51fe0a4ae891ee/pycryptodomex-3.17-cp27-cp27m-manylinux2014_aarch64.whl", hash = "sha256:db23d7341e21b273d2440ec6faf6c8b1ca95c8894da612e165be0b89a8688340"},
-    {url = "https://files.pythonhosted.org/packages/ac/a4/b2758579debd57abf5482a1f2f3a2a36c815fba9d6252fcd7fb5a7946aa7/pycryptodomex-3.17-cp35-abi3-win_amd64.whl", hash = "sha256:4b51e826f0a04d832eda0790bbd0665d9bfe73e5a4d8ea93b6a9b38beeebe935"},
-    {url = "https://files.pythonhosted.org/packages/ad/0b/df72e0e8d88a5292af108ae54c80dda7fbf034ca574906b574950608320d/pycryptodomex-3.17-cp27-cp27mu-manylinux2014_aarch64.whl", hash = "sha256:7a8dc3ee7a99aae202a4db52de5a08aa4d01831eb403c4d21da04ec2f79810db"},
-    {url = "https://files.pythonhosted.org/packages/ae/ad/c18d2eac9bf8053127146e0227bec0cd0a44e15fe51664c79cef11c8bf35/pycryptodomex-3.17-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:40e8a11f578bd0851b02719c862d55d3ee18d906c8b68a9c09f8c564d6bb5b92"},
-    {url = "https://files.pythonhosted.org/packages/b9/3b/0f4901806612cb9c9a20586c268f1b98497c6a65bd39dbc0ff7bb6694201/pycryptodomex-3.17-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:c84689c73358dfc23f9fdcff2cb9e7856e65e2ce3b5ed8ff630d4c9bdeb1867b"},
-    {url = "https://files.pythonhosted.org/packages/ba/e2/04a226505909388ec86c2bdd70c1199c575873e20591913bcec1439a2445/pycryptodomex-3.17-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:12056c38e49d972f9c553a3d598425f8a1c1d35b2e4330f89d5ff1ffb70de041"},
-    {url = "https://files.pythonhosted.org/packages/d1/72/d9ed0f68dfdd7322c3e0e4bcb0139b172bb66159dd2a5a95c6e2ce6f7a23/pycryptodomex-3.17-cp27-cp27m-musllinux_1_1_aarch64.whl", hash = "sha256:f854c8476512cebe6a8681cc4789e4fcff6019c17baa0fd72b459155dc605ab4"},
-    {url = "https://files.pythonhosted.org/packages/da/5f/4b904abe20347c88df413533ac88ad813e049639cc7e356673c8fe5fa450/pycryptodomex-3.17-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:caa937ff29d07a665dfcfd7a84f0d4207b2ebf483362fa9054041d67fdfacc20"},
+"pycryptodome 3.18.0" = [
+    {url = "https://files.pythonhosted.org/packages/02/50/e1cc5f1f0817af58d175cdad50f3ff7ae1490564803e6c625f4bd3c35e92/pycryptodome-3.18.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:9c8eda4f260072f7dbe42f473906c659dcbadd5ae6159dfb49af4da1293ae380"},
+    {url = "https://files.pythonhosted.org/packages/02/93/4822844082b641e7d1983e4a7e8eb1fa4ed206d7af182404cd1cd7fb10d5/pycryptodome-3.18.0-cp35-abi3-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4944defabe2ace4803f99543445c27dd1edbe86d7d4edb87b256476a91e9ffa4"},
+    {url = "https://files.pythonhosted.org/packages/0d/27/1fb1d3d7fe3e6af2586b7e4a4a24c687a1f5cacdd82e435fd62bd4fb6af0/pycryptodome-3.18.0-cp35-abi3-manylinux2014_aarch64.whl", hash = "sha256:10da29526a2a927c7d64b8f34592f461d92ae55fc97981aab5bbcde8cb465bb6"},
+    {url = "https://files.pythonhosted.org/packages/0f/26/7e4c213f49adc4b15d3518d6c6cc0e23f6234753303cdebbb8e22fb328fd/pycryptodome-3.18.0-cp35-abi3-win32.whl", hash = "sha256:795bd1e4258a2c689c0b1f13ce9684fa0dd4c0e08680dcf597cf9516ed6bc0f3"},
+    {url = "https://files.pythonhosted.org/packages/14/c2/6dead54adc193a5d30b6c54f6a048f56eb676bcbc8417f65156318d76d43/pycryptodome-3.18.0-cp27-cp27m-win_amd64.whl", hash = "sha256:16bfd98dbe472c263ed2821284118d899c76968db1a6665ade0c46805e6b29a4"},
+    {url = "https://files.pythonhosted.org/packages/1c/e1/2b88554ba22d89db6f9d62b5c1cb64098d9fdb6b1108c0fa1f3c8c9cd8af/pycryptodome-3.18.0-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:6f4b967bb11baea9128ec88c3d02f55a3e338361f5e4934f5240afcb667fdaec"},
+    {url = "https://files.pythonhosted.org/packages/20/1f/b5f4685d9bfb83fe052ea7f79413827af0c8a7b4672074d08f9918dbe44c/pycryptodome-3.18.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3811e31e1ac3069988f7a1c9ee7331b942e605dfc0f27330a9ea5997e965efb2"},
+    {url = "https://files.pythonhosted.org/packages/2c/bb/bfbb160bc50455767178192eed66dc595912ba24c09551fe908c5269019d/pycryptodome-3.18.0-cp35-abi3-macosx_10_9_x86_64.whl", hash = "sha256:53aee6be8b9b6da25ccd9028caf17dcdce3604f2c7862f5167777b707fbfb6cb"},
+    {url = "https://files.pythonhosted.org/packages/38/ee/99d66c28b2baf40a68053191e4f99ffd62639000efe7cc799f75843164c4/pycryptodome-3.18.0-cp35-abi3-musllinux_1_1_i686.whl", hash = "sha256:83c75952dcf4a4cebaa850fa257d7a860644c70a7cd54262c237c9f2be26f76e"},
+    {url = "https://files.pythonhosted.org/packages/3b/cb/4090eca51c31a1c7f6733d8d9a6ab96bc3e4559db6b57ec38372f554a037/pycryptodome-3.18.0-cp27-cp27mu-musllinux_1_1_aarch64.whl", hash = "sha256:422c89fd8df8a3bee09fb8d52aaa1e996120eafa565437392b781abec2a56e14"},
+    {url = "https://files.pythonhosted.org/packages/3f/a1/72ad8fbeb2630e74fa89622ab24ec0ce46dc93dc172156f1a112eb76c014/pycryptodome-3.18.0-cp35-abi3-win_amd64.whl", hash = "sha256:b1d9701d10303eec8d0bd33fa54d44e67b8be74ab449052a8372f12a66f93fb9"},
+    {url = "https://files.pythonhosted.org/packages/40/88/89623388754162ddb82c62814ccbfdbfcc8ed9bd6d5f7412d2479bdca3a7/pycryptodome-3.18.0-cp35-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f21efb8438971aa16924790e1c3dba3a33164eb4000106a55baaed522c261acf"},
+    {url = "https://files.pythonhosted.org/packages/5a/a8/05c3d516b489677d760c1855513bd87d85075c29382b58ccc8784a5c5724/pycryptodome-3.18.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:4604816adebd4faf8810782f137f8426bf45fee97d8427fa8e1e49ea78a52e2c"},
+    {url = "https://files.pythonhosted.org/packages/68/32/4309e91f5381793e2cdc0dfadefb298c78d2f4d4469a12b956331dca0579/pycryptodome-3.18.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:363dd6f21f848301c2dcdeb3c8ae5f0dee2286a5e952a0f04954b82076f23825"},
+    {url = "https://files.pythonhosted.org/packages/74/ac/f8cfa882380540f563df0d994c25c22d9296bcc9e56d2faab0f089448ec8/pycryptodome-3.18.0-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:78d863476e6bad2a592645072cc489bb90320972115d8995bcfbee2f8b209918"},
+    {url = "https://files.pythonhosted.org/packages/7a/ce/23ccf1f19bfaba114bfba068955ea78f7c511fb2fe5e4d89e920781bba7a/pycryptodome-3.18.0-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:12600268763e6fec3cefe4c2dcdf79bde08d0b6dc1813887e789e495cb9f3403"},
+    {url = "https://files.pythonhosted.org/packages/89/2b/4113d7124603ca258ba874633f1410760771c5313dfd73931fef4f272d63/pycryptodome-3.18.0-cp35-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:51eae079ddb9c5f10376b4131be9589a6554f6fd84f7f655180937f611cd99a2"},
+    {url = "https://files.pythonhosted.org/packages/8b/ed/572063febe91fb25efb4bb7ff2cc8b94604be25ce2482f3805d79495e404/pycryptodome-3.18.0-cp27-cp27m-musllinux_1_1_aarch64.whl", hash = "sha256:e8ad74044e5f5d2456c11ed4cfd3e34b8d4898c0cb201c4038fe41458a82ea27"},
+    {url = "https://files.pythonhosted.org/packages/92/d7/df2bf45a1bcc7f2983a22c05f77ecd04bb8252a734219b0a6f089121dfa3/pycryptodome-3.18.0-cp35-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:957b221d062d5752716923d14e0926f47670e95fead9d240fa4d4862214b9b2f"},
+    {url = "https://files.pythonhosted.org/packages/96/ad/98adb578b2d6de8db25f83933f9002803896e0d9df6897bfdef7d9a4a9d3/pycryptodome-3.18.0-pp27-pypy_73-manylinux2010_x86_64.whl", hash = "sha256:cb1be4d5af7f355e7d41d36d8eec156ef1382a88638e8032215c215b82a4b8ec"},
+    {url = "https://files.pythonhosted.org/packages/9c/ae/52cec7eecd8933c73909551c4c67517ca6deae16048857213b2ec28c0792/pycryptodome-3.18.0-cp27-cp27m-win32.whl", hash = "sha256:62a1e8847fabb5213ccde38915563140a5b338f0d0a0d363f996b51e4a6165cf"},
+    {url = "https://files.pythonhosted.org/packages/9d/dd/9927d01a8991c11d9a1cfecca3d293f9d6aa97cb51a472bc1b346819874a/pycryptodome-3.18.0-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:f022a4fd2a5263a5c483a2bb165f9cb27f2be06f2f477113783efe3fe2ad887b"},
+    {url = "https://files.pythonhosted.org/packages/a1/eb/030d2f273902f2b0c7d59bca28fe528dcc7213f2ddd5a65055a3f25101be/pycryptodome-3.18.0-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:d1497a8cd4728db0e0da3c304856cb37c0c4e3d0b36fcbabcc1600f18504fc54"},
+    {url = "https://files.pythonhosted.org/packages/ac/bb/54da82da28a437f41df1d807dfa9492d2afb670191d078f7ac6781a6f56e/pycryptodome-3.18.0-pp27-pypy_73-win32.whl", hash = "sha256:fc0a73f4db1e31d4a6d71b672a48f3af458f548059aa05e83022d5f61aac9c08"},
+    {url = "https://files.pythonhosted.org/packages/ad/0a/d050702d7db88ede0ce4792310dd8562656b8a38881714eb859f1634327b/pycryptodome-3.18.0-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:01489bbdf709d993f3058e2996f8f40fee3f0ea4d995002e5968965fa2fe89fb"},
+    {url = "https://files.pythonhosted.org/packages/b9/05/0e7547c445bbbc96c538d870e6c5c5a69a9fa5df0a9df3e27cb126527196/pycryptodome-3.18.0.tar.gz", hash = "sha256:c9adee653fc882d98956e33ca2c1fb582e23a8af7ac82fee75bd6113c55a0413"},
+    {url = "https://files.pythonhosted.org/packages/ce/62/eeb81dc5c95b79a92a95aaf7c0182a41d8d1d667f98a7dc35d6919f3ede5/pycryptodome-3.18.0-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:157c9b5ba5e21b375f052ca78152dd309a09ed04703fd3721dce3ff8ecced148"},
+    {url = "https://files.pythonhosted.org/packages/cf/93/bda6a6f0c32747de9451f9e183ff4b9dde7d6ffa4e798fd45007e4827563/pycryptodome-3.18.0-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:7a3d22c8ee63de22336679e021c7f2386f7fc465477d59675caa0e5706387944"},
+    {url = "https://files.pythonhosted.org/packages/e6/14/7451d35d7bc8153e4505e683782b1d110190a51626aa944d46caf78d3ebc/pycryptodome-3.18.0-cp27-cp27m-manylinux2014_aarch64.whl", hash = "sha256:d20082bdac9218649f6abe0b885927be25a917e29ae0502eaf2b53f1233ce0c2"},
+    {url = "https://files.pythonhosted.org/packages/ea/a8/79c30c277edae8450c28a18b33f0499414f023b1f45b75c6ea5f738f0955/pycryptodome-3.18.0-cp35-abi3-macosx_10_9_universal2.whl", hash = "sha256:9ad6f09f670c466aac94a40798e0e8d1ef2aa04589c29faa5b9b97566611d1d1"},
+    {url = "https://files.pythonhosted.org/packages/f5/9e/357a906a04c3c5d93f9f123de67a230681897cff3b3d87e4f8a337b412e2/pycryptodome-3.18.0-cp27-cp27mu-manylinux2014_aarch64.whl", hash = "sha256:b6a610f8bfe67eab980d6236fdc73bfcdae23c9ed5548192bb2d530e8a92780e"},
+    {url = "https://files.pythonhosted.org/packages/fd/31/39f22e64766c312b1d5af90c6f1bd7baa52fbde34d4c1c34cfdaa4be9b05/pycryptodome-3.18.0-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:928078c530da78ff08e10eb6cada6e0dff386bf3d9fa9871b4bbc9fbc1efe024"},
+]
+"pycryptodomex 3.18.0" = [
+    {url = "https://files.pythonhosted.org/packages/04/9f/48b22627934a89ceec72ef825eb121c17ec92c009045875fc0f2d10c1081/pycryptodomex-3.18.0-cp35-abi3-win32.whl", hash = "sha256:d56c9ec41258fd3734db9f5e4d2faeabe48644ba9ca23b18e1839b3bdf093222"},
+    {url = "https://files.pythonhosted.org/packages/06/19/c30ba6a73922541a8bb37dec97546b7bbb28277e88ff31f3f3856c3aebc2/pycryptodomex-3.18.0-cp27-cp27m-win32.whl", hash = "sha256:50308fcdbf8345e5ec224a5502b4215178bdb5e95456ead8ab1a69ffd94779cb"},
+    {url = "https://files.pythonhosted.org/packages/0a/e9/b2cd9bc1035f032d36b2400024c718b0a0b07214056a24e519b53a2a3b7a/pycryptodomex-3.18.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d35a8ffdc8b05e4b353ba281217c8437f02c57d7233363824e9d794cf753c419"},
+    {url = "https://files.pythonhosted.org/packages/11/8d/6681e86a5640923f9ac029951df69e98857a53ddc436b661f6514d0d1205/pycryptodomex-3.18.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:215be2980a6b70704c10796dd7003eb4390e7be138ac6fb8344bf47e71a8d470"},
+    {url = "https://files.pythonhosted.org/packages/15/63/1029901f16d01298cf77e7d130b8bbd2aeeefac189009dee350a563a11d7/pycryptodomex-3.18.0-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:76f0a46bee539dae4b3dfe37216f678769349576b0080fdbe431d19a02da42ff"},
+    {url = "https://files.pythonhosted.org/packages/15/bf/392fefeacbc2bdf91eabf893daa92ade1804b631a516e189e833b3f06c6d/pycryptodomex-3.18.0-cp35-abi3-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:6875eb8666f68ddbd39097867325bd22771f595b4e2b0149739b5623c8bf899b"},
+    {url = "https://files.pythonhosted.org/packages/16/49/474341bfa056ab417bb3881d9d761d1ad8e7e93e80dc7f323c26dfd28ccc/pycryptodomex-3.18.0-pp27-pypy_73-manylinux2010_x86_64.whl", hash = "sha256:2dc4eab20f4f04a2d00220fdc9258717b82d31913552e766d5f00282c031b70a"},
+    {url = "https://files.pythonhosted.org/packages/1a/0c/1b35461d7091e074d2c393face4768cb99844174dd858ac98e5044ca14ac/pycryptodomex-3.18.0-cp35-abi3-manylinux2014_aarch64.whl", hash = "sha256:6421d23d6a648e83ba2670a352bcd978542dad86829209f59d17a3f087f4afef"},
+    {url = "https://files.pythonhosted.org/packages/1a/32/816f7fa43e1af0b6f43f224d0dbcc8204e7365a8e3f9eccd06c690d70ccd/pycryptodomex-3.18.0-cp27-cp27m-musllinux_1_1_aarch64.whl", hash = "sha256:f9ab5ef0718f6a8716695dea16d83b671b22c45e9c0c78fd807c32c0192e54b5"},
+    {url = "https://files.pythonhosted.org/packages/1b/da/f8bde80db24989614622d8f13ae3788343bf599e612d96b9b8f8452f5bd9/pycryptodomex-3.18.0-cp27-cp27mu-manylinux2014_aarch64.whl", hash = "sha256:3d9314ac785a5b75d5aaf924c5f21d6ca7e8df442e5cf4f0fefad4f6e284d422"},
+    {url = "https://files.pythonhosted.org/packages/40/92/efd675dba957315d705f792b28d900bddc36f39252f6713961b4221ee9af/pycryptodomex-3.18.0.tar.gz", hash = "sha256:3e3ecb5fe979e7c1bb0027e518340acf7ee60415d79295e5251d13c68dde576e"},
+    {url = "https://files.pythonhosted.org/packages/45/09/ce11344724e674957402b5f3c0d663388f755ecd1c864f0c405b5f959bd8/pycryptodomex-3.18.0-cp35-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d84e105787f5e5d36ec6a581ff37a1048d12e638688074b2a00bcf402f9aa1c2"},
+    {url = "https://files.pythonhosted.org/packages/46/e6/7dbe57f21195e9f85c4d77ae995aa2a39dc45a2e34a978d98099c6ed43ce/pycryptodomex-3.18.0-cp35-abi3-macosx_10_9_universal2.whl", hash = "sha256:ac614363a86cc53d8ba44b6c469831d1555947e69ab3276ae8d6edc219f570f7"},
+    {url = "https://files.pythonhosted.org/packages/47/fc/e94343fc7fbffb5eec5a96ca2d92f7cc4c970f4618bf152c7054c3e9b0bd/pycryptodomex-3.18.0-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:73d64b32d84cf48d9ec62106aa277dbe99ab5fbfd38c5100bc7bddd3beb569f7"},
+    {url = "https://files.pythonhosted.org/packages/4a/9d/d8e412629a4f55338cf60567bac2e0acccd021979f1d75d693b1e3a64020/pycryptodomex-3.18.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:71687eed47df7e965f6e0bf3cadef98f368d5221f0fb89d2132effe1a3e6a194"},
+    {url = "https://files.pythonhosted.org/packages/5f/aa/84f77b251353ec0494fe5fa118fa95462f2edc9413e34f451a504e1f43e0/pycryptodomex-3.18.0-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:c2953afebf282a444c51bf4effe751706b4d0d63d7ca2cc51db21f902aa5b84e"},
+    {url = "https://files.pythonhosted.org/packages/5f/e6/958e5ccdfeeee3e984a505d66787b29fa557c56155358f0d4199a7cb6a70/pycryptodomex-3.18.0-cp27-cp27m-manylinux2014_aarch64.whl", hash = "sha256:192306cf881fe3467dda0e174a4f47bb3a8bb24b90c9cdfbdc248eec5fc0578c"},
+    {url = "https://files.pythonhosted.org/packages/6d/e5/56c1479ccefa96551b46d07c8881c202c9be0ccda1ffd957a032c1306940/pycryptodomex-3.18.0-cp35-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:6ed3606832987018615f68e8ed716a7065c09a0fe94afd7c9ca1b6777f0ac6eb"},
+    {url = "https://files.pythonhosted.org/packages/73/c1/080fcc7d0a7e25808e9cd8814d543e8f80466ce476003fe17e109deae568/pycryptodomex-3.18.0-pp27-pypy_73-win32.whl", hash = "sha256:75672205148bdea34669173366df005dbd52be05115e919551ee97171083423d"},
+    {url = "https://files.pythonhosted.org/packages/78/99/cb6e8abdca42ec6b6bfcd5c0ee6376936addc4844d45d30c53b6a5511087/pycryptodomex-3.18.0-cp35-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:27072a494ce621cc7a9096bbf60ed66826bb94db24b49b7359509e7951033e74"},
+    {url = "https://files.pythonhosted.org/packages/7c/6f/fdf4620511f30482915c88cba42e82b2ce3444499bfeba572c16abfd22e6/pycryptodomex-3.18.0-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:160a39a708c36fa0b168ab79386dede588e62aec06eb505add870739329aecc6"},
+    {url = "https://files.pythonhosted.org/packages/86/b4/cee6a2153e0614b7b4ab476ab64827281057e49cb357d736ab986190b20b/pycryptodomex-3.18.0-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:5594a125dae30d60e94f37797fc67ce3c744522de7992c7c360d02fdb34918f8"},
+    {url = "https://files.pythonhosted.org/packages/8a/db/12a08d50aa8586c2e32b2b4461b89c0de057d1c637a13ac8b785dfd55327/pycryptodomex-3.18.0-cp35-abi3-win_amd64.whl", hash = "sha256:e00a4bacb83a2627e8210cb353a2e31f04befc1155db2976e5e239dd66482278"},
+    {url = "https://files.pythonhosted.org/packages/8b/7a/deb0fe034b43157077d780099a81709bedc785f28096cac99cf051c13711/pycryptodomex-3.18.0-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:ba95abd563b0d1b88401658665a260852a8e6c647026ee6a0a65589287681df8"},
+    {url = "https://files.pythonhosted.org/packages/8d/2e/c1433abaa4335a0c668ff93fd57f714436ec6107eeff1f43f456011b2b27/pycryptodomex-3.18.0-cp35-abi3-musllinux_1_1_i686.whl", hash = "sha256:1949e09ea49b09c36d11a951b16ff2a05a0ffe969dda1846e4686ee342fe8646"},
+    {url = "https://files.pythonhosted.org/packages/8f/ad/8a6ace1d145c6e699477a3f71f5a5183c922182d1bf1411bbc2bf918914d/pycryptodomex-3.18.0-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:bec6c80994d4e7a38312072f89458903b65ec99bed2d65aa4de96d997a53ea7a"},
+    {url = "https://files.pythonhosted.org/packages/a7/c0/8ecbd1cecc470a4aed2e5b69db367de5f87692d6d40e604b5dae58b77ed6/pycryptodomex-3.18.0-cp35-abi3-macosx_10_9_x86_64.whl", hash = "sha256:302a8f37c224e7b5d72017d462a2be058e28f7be627bdd854066e16722d0fc0c"},
+    {url = "https://files.pythonhosted.org/packages/b5/48/0dcad9903dc331169f4ba8bf60e5a81c41d3725ae5ccca20f590269641f5/pycryptodomex-3.18.0-cp27-cp27mu-musllinux_1_1_aarch64.whl", hash = "sha256:f237278836dda412a325e9340ba2e6a84cb0f56b9244781e5b61f10b3905de88"},
+    {url = "https://files.pythonhosted.org/packages/b9/76/dae6bec36fa6a36d2579d99fc64f67038aa112598eed1fe35315332474f5/pycryptodomex-3.18.0-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:58fc0aceb9c961b9897facec9da24c6a94c5db04597ec832060f53d4d6a07196"},
+    {url = "https://files.pythonhosted.org/packages/bd/29/e1145ac172a3cc0ec70d2857ea919f87430d3f2b0727022b8f4329527faa/pycryptodomex-3.18.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bbdcce0a226d9205560a5936b05208c709b01d493ed8307792075dedfaaffa5f"},
+    {url = "https://files.pythonhosted.org/packages/ef/1a/1ce7e65be28111cf6115a968516074f486edf7daa5d351cb2e7269698f84/pycryptodomex-3.18.0-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:8ff129a5a0eb5ff16e45ca4fa70a6051da7f3de303c33b259063c19be0c43d35"},
+    {url = "https://files.pythonhosted.org/packages/f6/9f/ab0bf98fbbf4f1ee8751566b8fc6e1613c856c81f1a887736e6f2959db8e/pycryptodomex-3.18.0-cp27-cp27m-win_amd64.whl", hash = "sha256:4d9379c684efea80fdab02a3eb0169372bca7db13f9332cb67483b8dc8b67c37"},
+]
+"pydantic 1.10.8" = [
+    {url = "https://files.pythonhosted.org/packages/05/43/e39c6bf32695f2d568ebb2f6a3dd843c8e2edb57c77a4a911d517b5675b2/pydantic-1.10.8-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:35db5301b82e8661fa9c505c800d0990bc14e9f36f98932bb1d248c0ac5cada5"},
+    {url = "https://files.pythonhosted.org/packages/0b/39/afbca0ea8e766ccf04f224520b95ca29d5a18b680c0780609a2c39293f8b/pydantic-1.10.8-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:1243d28e9b05003a89d72e7915fdb26ffd1d39bdd39b00b7dbe4afae4b557f9d"},
+    {url = "https://files.pythonhosted.org/packages/13/dc/54ceed364e733f81596a4f113de2098221b3d39b4eb7abbffa64e681f243/pydantic-1.10.8-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:666bdf6066bf6dbc107b30d034615d2627e2121506c555f73f90b54a463d1f33"},
+    {url = "https://files.pythonhosted.org/packages/15/27/c35f6fefc782aebcff9991b28728f3855b1253ff757e6dee8e3ac3815cd0/pydantic-1.10.8-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:191ba419b605f897ede9892f6c56fb182f40a15d309ef0142212200a10af4c18"},
+    {url = "https://files.pythonhosted.org/packages/23/65/2aa13873e9e0084ecaec00fbe6c6096b65e1ab99ba66bdbf7e4e7c4cc915/pydantic-1.10.8.tar.gz", hash = "sha256:1410275520dfa70effadf4c21811d755e7ef9bb1f1d077a21958153a92c8d9ca"},
+    {url = "https://files.pythonhosted.org/packages/2d/a2/e3ac01dd929485a6280518d280d8cf313558c878c91d86b3a95b1702938b/pydantic-1.10.8-cp310-cp310-win_amd64.whl", hash = "sha256:ab523c31e22943713d80d8d342d23b6f6ac4b792a1e54064a8d0cf78fd64e800"},
+    {url = "https://files.pythonhosted.org/packages/36/60/b24bd42bdd385fee681cc1231ef1d423566d4e33e867df4d2bd08b531466/pydantic-1.10.8-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6f2e754d5566f050954727c77f094e01793bcb5725b663bf628fa6743a5a9108"},
+    {url = "https://files.pythonhosted.org/packages/56/b5/903cd28ab9a3bf8cbfbe0a6a87d9463ceac7610193cd1d72bb1bdb276d01/pydantic-1.10.8-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f90c1e29f447557e9e26afb1c4dbf8768a10cc676e3781b6a577841ade126b85"},
+    {url = "https://files.pythonhosted.org/packages/57/ce/b3de85c397a03f1c8dadebe33fa81b195b6090c840a0333769fba00693fd/pydantic-1.10.8-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:1952526ba40b220b912cdc43c1c32bcf4a58e3f192fa313ee665916b26befb68"},
+    {url = "https://files.pythonhosted.org/packages/59/ab/1de0d5386a464ef527338d320216a2f41de416e204780e00baa0e5e3b807/pydantic-1.10.8-cp38-cp38-win_amd64.whl", hash = "sha256:6a82d6cda82258efca32b40040228ecf43a548671cb174a1e81477195ed3ed56"},
+    {url = "https://files.pythonhosted.org/packages/6b/15/3504de0fcb90336680916ea3fde845d01fa846c95ab4342c28d985c0d29d/pydantic-1.10.8-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:93e766b4a8226e0708ef243e843105bf124e21331694367f95f4e3b4a92bbb3f"},
+    {url = "https://files.pythonhosted.org/packages/6c/32/0755046e707a468fe276fd40df11d492a72d1cbcfa344091e3a46120131c/pydantic-1.10.8-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c0ab53b609c11dfc0c060d94335993cc2b95b2150e25583bec37a49b2d6c6c3f"},
+    {url = "https://files.pythonhosted.org/packages/6c/f9/5edecae1914fc7dc6a566809a5242c97d63acfb92253b0bb885d890eb953/pydantic-1.10.8-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:42aa0c4b5c3025483240a25b09f3c09a189481ddda2ea3a831a9d25f444e03c1"},
+    {url = "https://files.pythonhosted.org/packages/6f/4d/7647a5f98fbcbb9bdb1e5a77eca931a1f83255c9aa14448794a0596b5a42/pydantic-1.10.8-cp37-cp37m-win_amd64.whl", hash = "sha256:16f8c3e33af1e9bb16c7a91fc7d5fa9fe27298e9f299cff6cb744d89d573d62c"},
+    {url = "https://files.pythonhosted.org/packages/77/ea/2b96534811f867bb53edaf2a3ca5037d8bcbceb05d5930bac5caa1fba573/pydantic-1.10.8-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1ced8375969673929809d7f36ad322934c35de4af3b5e5b09ec967c21f9f7887"},
+    {url = "https://files.pythonhosted.org/packages/7a/ba/439e2bc693d3f464946159a76724efc570cef9f4e27303fa3b360b2f3ef7/pydantic-1.10.8-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ceb6a23bf1ba4b837d0cfe378329ad3f351b5897c8d4914ce95b85fba96da5a1"},
+    {url = "https://files.pythonhosted.org/packages/98/20/52707fc7dc91b6e580dbd30c4a6b88e426f61af9f2547bb52e880f09e67d/pydantic-1.10.8-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:12f7b0bf8553e310e530e9f3a2f5734c68699f42218bf3568ef49cd9b0e44df4"},
+    {url = "https://files.pythonhosted.org/packages/a7/27/80672dfb14e47293cca421580141ec923a1e5fe7283f775079e006b0be28/pydantic-1.10.8-cp311-cp311-win_amd64.whl", hash = "sha256:d532bf00f381bd6bc62cabc7d1372096b75a33bc197a312b03f5838b4fb84edd"},
+    {url = "https://files.pythonhosted.org/packages/b2/43/8eca9ebbfd861209365c5b9f982b113275eccd892e53ab7bde60a21439e8/pydantic-1.10.8-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:34d327c81e68a1ecb52fe9c8d50c8a9b3e90d3c8ad991bfc8f953fb477d42fb4"},
+    {url = "https://files.pythonhosted.org/packages/b8/45/538d65960c489a1aa9cbf1f54d4b911e1e838d557d2d2ccd1b6c8fa10f3b/pydantic-1.10.8-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:17aef11cc1b997f9d574b91909fed40761e13fac438d72b81f902226a69dac01"},
+    {url = "https://files.pythonhosted.org/packages/c1/37/d136df986c0a2d20f940d360fe472ae410fba46f55a73e872fd3168f4289/pydantic-1.10.8-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:0c6fafa0965b539d7aab0a673a046466d23b86e4b0e8019d25fd53f4df62c277"},
+    {url = "https://files.pythonhosted.org/packages/c4/f3/c5dc9f49783a6407487d20c9a32bca878ebf2df155b8d2858838d79b6d46/pydantic-1.10.8-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:bb14388ec45a7a0dc429e87def6396f9e73c8c77818c927b6a60706603d5f2ea"},
+    {url = "https://files.pythonhosted.org/packages/c5/58/71d48d4154e5845192f4ccc6c6ebcf6fa5286fa3bcb3c595aa18a5bf599d/pydantic-1.10.8-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:e82d4566fcd527eae8b244fa952d99f2ca3172b7e97add0b43e2d97ee77f81ab"},
+    {url = "https://files.pythonhosted.org/packages/ca/5b/8b2c49589c826bf2796fc523d77d46fed2e82585c87c812f289ce244c88b/pydantic-1.10.8-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2e4148e635994d57d834be1182a44bdb07dd867fa3c2d1b37002000646cc5459"},
+    {url = "https://files.pythonhosted.org/packages/cc/a4/354a73bb8a06df0df0bc74b5fbf3b9510ed4900185f86a00861dcfbe60c7/pydantic-1.10.8-py3-none-any.whl", hash = "sha256:7456eb22ed9aaa24ff3e7b4757da20d9e5ce2a81018c1b3ebd81a0b88a18f3b2"},
+    {url = "https://files.pythonhosted.org/packages/d8/7b/ca035af1833c6d047eeb328438a2ae402d03929be2055cd66294542a814d/pydantic-1.10.8-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:052d8654cb65174d6f9490cc9b9a200083a82cf5c3c5d3985db765757eb3b375"},
+    {url = "https://files.pythonhosted.org/packages/dc/92/3a09ec18592ca6fc96223b42ad20c8711847a8d2e1800779f9206c2fa6a2/pydantic-1.10.8-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:df7800cb1984d8f6e249351139667a8c50a379009271ee6236138a22a0c0f319"},
+    {url = "https://files.pythonhosted.org/packages/e2/21/e6f68631ec2f0470e28722d1ca352bac4f25aef6eb18b8e65ba3cd9ae8a2/pydantic-1.10.8-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7b1f6cb446470b7ddf86c2e57cd119a24959af2b01e552f60705910663af09a4"},
+    {url = "https://files.pythonhosted.org/packages/e6/dd/6f9ef794df128746581bd5886c6382a19f1729ff39f3d65e66e3b6751c7a/pydantic-1.10.8-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c33b60054b2136aef8cf190cd4c52a3daa20b2263917c49adad20eaf381e823b"},
+    {url = "https://files.pythonhosted.org/packages/e7/a3/329824b0e46edcb2c51f0fa73678f24aba083289697a0db3036f4f30e1ed/pydantic-1.10.8-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3e59417ba8a17265e632af99cc5f35ec309de5980c440c255ab1ca3ae96a3e0e"},
+    {url = "https://files.pythonhosted.org/packages/e8/b3/b748afd5f4fd8f640e08cf4828fa5c9da865353eade18b9c789726b1a0ce/pydantic-1.10.8-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f9613fadad06b4f3bc5db2653ce2f22e0de84a7c6c293909b48f6ed37b83c61f"},
+    {url = "https://files.pythonhosted.org/packages/e9/17/a840d0631a288a4400e23a9ec96d131bd07be820fe2c1d070995de6dfb61/pydantic-1.10.8-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:93e6bcfccbd831894a6a434b0aeb1947f9e70b7468f274154d03d71fabb1d7c6"},
+    {url = "https://files.pythonhosted.org/packages/fa/3b/279a13153350b688fb5eb557acf980059a21ffede20d9b6fbc5368778bf4/pydantic-1.10.8-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:84d80219c3f8d4cad44575e18404099c76851bc924ce5ab1c4c8bb5e2a2227d0"},
+    {url = "https://files.pythonhosted.org/packages/fb/46/723587abb4aecf82edcfaa213a827d61854ebcbf76b4818cbf59c8868f4e/pydantic-1.10.8-cp39-cp39-win_amd64.whl", hash = "sha256:66a703d1983c675a6e0fed8953b0971c44dba48a929a2000a493c3772eb61a5a"},
+    {url = "https://files.pythonhosted.org/packages/fe/26/66c9ac1e21a3bda4f5c10785b3ff199e12e2d1e984780a8bfa796bb4e2f0/pydantic-1.10.8-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:7d5b8641c24886d764a74ec541d2fc2c7fb19f6da2a4001e6d580ba4a38f7878"},
+    {url = "https://files.pythonhosted.org/packages/ff/b4/b56bd5f591969df63a260555a891bf953536eefcbe66b711b80f86acc3a4/pydantic-1.10.8-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:88f195f582851e8db960b4a94c3e3ad25692c1c1539e2552f3df7a9e972ef60e"},
 ]
 "pyexiftool 0.5.5" = [
     {url = "https://files.pythonhosted.org/packages/78/04/10ac8e25bfbfd6297194e1fefdeaba1cc981ae2f5a36dd03ba30db3bbee0/PyExifTool-0.5.5.tar.gz", hash = "sha256:9dce4638c1d4d1b3414eb4e720647582f2ec14e940f97e42d4ba202580e04a66"},
     {url = "https://files.pythonhosted.org/packages/bd/fb/ffb698a0e3d8e1f45a051be009b6dd4494bd665b165ec28c594bb535cec7/PyExifTool-0.5.5-py3-none-any.whl", hash = "sha256:7048aab1cb83726d7bf0113a5acb9d9d52f9e16817e39595fa59c8ea0563bf5a"},
 ]
 "pygments 2.15.1" = [
     {url = "https://files.pythonhosted.org/packages/34/a7/37c8d68532ba71549db4212cb036dbd6161b40e463aba336770e80c72f84/Pygments-2.15.1-py3-none-any.whl", hash = "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"},
@@ -2542,32 +2898,32 @@
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
 "rich 13.3.5" = [
     {url = "https://files.pythonhosted.org/packages/39/03/6de23bdd88f5ee7f8b03f94f6e88108f5d7ffe6d207e95cdb06d9aa4cd57/rich-13.3.5-py3-none-any.whl", hash = "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"},
     {url = "https://files.pythonhosted.org/packages/3d/0b/8dd34d20929c4b5e474db2e64426175469c2b7fea5ba71c6d4b3397a9729/rich-13.3.5.tar.gz", hash = "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c"},
 ]
-"ruff 0.0.269" = [
-    {url = "https://files.pythonhosted.org/packages/02/65/c49103428b27ef3831f6f8023a062de07d7a88d4d9d9f22cbf4941331b4b/ruff-0.0.269-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:f062059b8289a4fab7f6064601b811d447c2f9d3d432a17f689efe4d68988450"},
-    {url = "https://files.pythonhosted.org/packages/18/f1/28f24e47a8dfb72762056713fd66c2f6fd543d0f6d3858291cb3d4993c2a/ruff-0.0.269-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1f19f59ca3c28742955241fb452f3346241ddbd34e72ac5cb3d84fadebcf6bc8"},
-    {url = "https://files.pythonhosted.org/packages/1d/97/60d69db70fa1e7e29a553fc6719ef6b750da0d570285f4c890ba686655f8/ruff-0.0.269-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6da8ee25ef2f0cc6cc8e6e20942c1d44d25a36dce35070d7184655bc14f63f63"},
-    {url = "https://files.pythonhosted.org/packages/26/64/3e1fc0ccf7d59d7c45ec643541642cd3bcc95c36b5c2e01f9f9f908650c4/ruff-0.0.269-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:cec2f4b84a14b87f1b121488649eb5b4eaa06467a2387373f750da74bdcb5679"},
-    {url = "https://files.pythonhosted.org/packages/2a/22/514380df775cac977caaa1394e2955c600e6f3895c0713e5f5aa99735d02/ruff-0.0.269-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3f5dc7aac52c58e82510217e3c7efd80765c134c097c2815d59e40face0d1fe6"},
-    {url = "https://files.pythonhosted.org/packages/30/ff/e1e0ec0e4e31b3f163ef3e80456150a41a3b910cac04472a13248b812ce6/ruff-0.0.269-py3-none-win_arm64.whl", hash = "sha256:bbeb857b1e508a4487bdb02ca1e6d41dd8d5ac5335a5246e25de8a3dff38c1ff"},
-    {url = "https://files.pythonhosted.org/packages/3c/42/88f5242e41988bb83a37a04f16f3523c4b65b2133fa5e9d05ef276dd0b70/ruff-0.0.269-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:5a20658f0b97d207c7841c13d528f36d666bf445b00b01139f28a8ccb80093bb"},
-    {url = "https://files.pythonhosted.org/packages/4a/04/77ad67155861ccf0deead144e4ba766b54c669c37aafc25d092a1a4f0af7/ruff-0.0.269.tar.gz", hash = "sha256:11ddcfbab32cf5c420ea9dd5531170ace5a3e59c16d9251c7bd2581f7b16f602"},
-    {url = "https://files.pythonhosted.org/packages/5b/93/67a13d30ae7d709774ab14b12ba6e90d3d8116a19afae1f0a5a818513ea1/ruff-0.0.269-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a374434e588e06550df0f8dcb74777290f285678de991fda4e1063c367ab2eb2"},
-    {url = "https://files.pythonhosted.org/packages/95/19/0c3372acb612100e7417e394b85d98e3a73d80c6cc5a86d0253a40bc68ca/ruff-0.0.269-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:374b161753a247904aec7a32d45e165302b76b6e83d22d099bf3ff7c232c888f"},
-    {url = "https://files.pythonhosted.org/packages/9c/38/1ce6bc423e9e86ed21e4cae62a0f67f08ddc8bfdadcd2c340e427fd3e9a1/ruff-0.0.269-py3-none-win_amd64.whl", hash = "sha256:f3b59ccff57b21ef0967ea8021fd187ec14c528ec65507d8bcbe035912050776"},
-    {url = "https://files.pythonhosted.org/packages/a9/a4/b555c6fb6880c64cd88e42e44c235770abf6263457ab493dac4ad123c427/ruff-0.0.269-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:bd81b8e681b9eaa6cf15484f3985bd8bd97c3d114e95bff3e8ea283bf8865062"},
-    {url = "https://files.pythonhosted.org/packages/b9/9f/692b03ed8f2065e4fd628d5f55ba68fe941cd23bd6f9afa4eddcba27316b/ruff-0.0.269-py3-none-win32.whl", hash = "sha256:03ff42bc91ceca58e0f0f072cb3f9286a9208f609812753474e799a997cdad1a"},
-    {url = "https://files.pythonhosted.org/packages/bf/0b/6415002df30de68a541f0fce1adb77d8160b5afb36edeea2e0c3fbf28192/ruff-0.0.269-py3-none-musllinux_1_2_i686.whl", hash = "sha256:9ca0a1ddb1d835b5f742db9711c6cf59f213a1ad0088cb1e924a005fd399e7d8"},
-    {url = "https://files.pythonhosted.org/packages/d4/7c/1b8378f80962ff7d129a39785964710f92ebd9fa91e2444f00635ba3f510/ruff-0.0.269-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:3569bcdee679045c09c0161fabc057599759c49219a08d9a4aad2cc3982ccba3"},
-    {url = "https://files.pythonhosted.org/packages/f6/0c/eced078f3e0a4461b10dbf163160bd7a860378303a07253cbe8d1541fff4/ruff-0.0.269-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:56347da63757a56cbce7d4b3d6044ca4f1941cd1bbff3714f7554360c3361f83"},
-    {url = "https://files.pythonhosted.org/packages/f8/17/90e1cb087a20e136da10b0187cf1bf25ac80da1c5fcb0256b683e6eee047/ruff-0.0.269-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e131b4dbe798c391090c6407641d6ab12c0fa1bb952379dde45e5000e208dabb"},
+"ruff 0.0.270" = [
+    {url = "https://files.pythonhosted.org/packages/02/d1/77f9425bea1e5a929ecbeb3fd9e2e0931e30751b4d75bbe8b46e14408ada/ruff-0.0.270-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:643de865fd35cb76c4f0739aea5afe7b8e4d40d623df7e9e6ea99054e5cead0a"},
+    {url = "https://files.pythonhosted.org/packages/06/56/39079c40dc7e995f26f630d28dec11b1b63f498bfb56409adda27300bf2f/ruff-0.0.270-py3-none-win_amd64.whl", hash = "sha256:0012f9b7dc137ab7f1f0355e3c4ca49b562baf6c9fa1180948deeb6648c52957"},
+    {url = "https://files.pythonhosted.org/packages/36/21/aa8e1d22756e1d3bcdb43f4d25451f8978cacd9d6896e365bb7c1f9037fa/ruff-0.0.270-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:08188f8351f4c0b6216e8463df0a76eb57894ca59a3da65e4ed205db980fd3ae"},
+    {url = "https://files.pythonhosted.org/packages/36/ab/ff2870e22556c780d6b0b2934152e824ca0d3d40d9e3dedb44a158a979dc/ruff-0.0.270-py3-none-musllinux_1_2_i686.whl", hash = "sha256:0bbfbf6fd2436165566ca85f6e57be03ed2f0a994faf40180cfbb3604c9232ef"},
+    {url = "https://files.pythonhosted.org/packages/40/82/c393794c4cd462ffbd0afe45b8e77c174c7f3d5df4340ecead9a42d1fa53/ruff-0.0.270-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:0827b074635d37984fc98d99316bfab5c8b1231bb83e60dacc83bd92883eedb4"},
+    {url = "https://files.pythonhosted.org/packages/57/2f/3f964a1d0208248f3c51441a9e59690c8ac6f33422a0f0918521743c9f16/ruff-0.0.270-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:0d61ae4841313f6eeb8292dc349bef27b4ce426e62c36e80ceedc3824e408734"},
+    {url = "https://files.pythonhosted.org/packages/5a/22/e4e4d9219993e3b7f34ba16b9b14176d19bc77232daf70d176ee86687d51/ruff-0.0.270-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:739495d2dbde87cf4e3110c8d27bc20febf93112539a968a4e02c26f0deccd1d"},
+    {url = "https://files.pythonhosted.org/packages/7f/2c/3989a9296e058720b65106bcb4756781ddada2c258fb2f54be0e702602cf/ruff-0.0.270-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:eca02e709b3308eb7255b5f74e779be23b5980fca3862eae28bb23069cd61ae4"},
+    {url = "https://files.pythonhosted.org/packages/9a/fb/625f83b6e19ef8d78f68cc43afdcb26f0e59ed83c3c569f7cdfa09afd276/ruff-0.0.270-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:21f00e47ab2308617c44435c8dfd9e2e03897461c9e647ec942deb2a235b4cfd"},
+    {url = "https://files.pythonhosted.org/packages/a6/fc/fd90a58b09ec004f773617a92e0844e30830791e9c6e39582fae414966c2/ruff-0.0.270-py3-none-win_arm64.whl", hash = "sha256:9613456b0b375766244c25045e353bc8890c856431cd97893c97b10cc93bd28d"},
+    {url = "https://files.pythonhosted.org/packages/af/a0/2b773726f2b534acc32ea60b51a3e2f0b130b68a67a32baa099536c153a4/ruff-0.0.270-py3-none-win32.whl", hash = "sha256:b4c037fe2f75bcd9aed0c89c7c507cb7fa59abae2bd4c8b6fc331a28178655a4"},
+    {url = "https://files.pythonhosted.org/packages/b0/6f/d875381e8ca1070b6065aad1095b5b7dff0a2b2198962f72166efd6bbf24/ruff-0.0.270.tar.gz", hash = "sha256:95db07b7850b30ebf32b27fe98bc39e0ab99db3985edbbf0754d399eb2f0e690"},
+    {url = "https://files.pythonhosted.org/packages/b2/4d/c74c7223aa96e2168aa55042a9123a41daddb585e1d492b10de45bcf4db9/ruff-0.0.270-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:b775e2c5fc869359daf8c8b8aa0fd67240201ab2e8d536d14a0edf279af18786"},
+    {url = "https://files.pythonhosted.org/packages/c0/90/cdbb101b1864aba6a785ef5a91c426abd4d76a3863054496c7c32a20ace8/ruff-0.0.270-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:f74c4d550f7b8e808455ac77bbce38daafc458434815ba0bc21ae4bdb276509b"},
+    {url = "https://files.pythonhosted.org/packages/cb/1e/c6aa0c7e443bae068fe151c592d07078dbb75efcc4c8d73fbf8a7f872e85/ruff-0.0.270-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0eb412f20e77529a01fb94d578b19dcb8331b56f93632aa0cce4a2ea27b7aeba"},
+    {url = "https://files.pythonhosted.org/packages/dc/59/4f1e078ddf622e42096a45e3e3e3dd524499557044847261e40817f56d2e/ruff-0.0.270-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:8af391ef81f7be960be10886a3c1aac0b298bde7cb9a86ec2b05faeb2081ce6b"},
+    {url = "https://files.pythonhosted.org/packages/f0/48/a56cdeec0277aff92d68c39c282c9f7c01f38db37c5832605ee8c1ed8097/ruff-0.0.270-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:3ed3b198768d2b3a2300fb18f730cd39948a5cc36ba29ae9d4639a11040880be"},
 ]
 "scalene 1.5.19" = [
     {url = "https://files.pythonhosted.org/packages/11/19/c973ecc43b18076df6c7efff7bec280d02d48d8245f46d94b7e90cf306f2/scalene-1.5.19-cp39-cp39-win_amd64.whl", hash = "sha256:d1fd5d83f3c022ddc46049f29823351b8dbdb8590f5803358fa6034784601f24"},
     {url = "https://files.pythonhosted.org/packages/19/54/d89426ab970f1cb3850b0374967ae22d831d0091efeb2c1d8e8d02ac2a19/scalene-1.5.19-cp39-cp39-macosx_11_7_universal2.whl", hash = "sha256:6c08f3bc0b6355db3c34f0e9aea1b291e64675bb832e19758ee751918787cac0"},
     {url = "https://files.pythonhosted.org/packages/49/11/5a2fa4567eee217609e0a627534f5fb60d0c1f768b43a93145a2ea24e39b/scalene-1.5.19-cp38-cp38-manylinux_2_24_x86_64.whl", hash = "sha256:f67f39321548c06de440319bdd70c41c14b6c50d4748226a101402995677cade"},
     {url = "https://files.pythonhosted.org/packages/5e/3c/b1f159a11f0949f3f27b18af1cc68ee301088a7337efc7d961684bdd3f46/scalene-1.5.19-cp37-cp37m-macosx_10_15_universal2.whl", hash = "sha256:58fb40d031081a55e813f292b2d85b64d7558a372832d8e456f7fe2113adf182"},
     {url = "https://files.pythonhosted.org/packages/65/c3/ebaf00eef807b8da6c5b0c4eb6627f0a67538a25ac7e3858347e15c55d22/scalene-1.5.19-cp38-cp38-win_amd64.whl", hash = "sha256:7a1d452ad4d32cf8adb8b86cae4e5b9c7bff866fff1c43618f9ad114b9ecac32"},
@@ -2582,36 +2938,115 @@
     {url = "https://files.pythonhosted.org/packages/f1/95/dae88019fcff89cc1cc3b6fc85b9fc3a25a264b21b67000a665dd3ae372a/scalene-1.5.19-cp310-cp310-win_amd64.whl", hash = "sha256:cdb9be734cfb6b42eef1105fee1876a5c465eb72e109c0d0ceea6e6bdbce21c6"},
     {url = "https://files.pythonhosted.org/packages/fb/08/ed0d55f81bc2bc261c922a2d4171360b1a3a5d6a4e57ccc640fb09a02706/scalene-1.5.19-cp39-cp39-manylinux_2_24_x86_64.whl", hash = "sha256:d8bc53334b13e486ed6ba03fe4b7595ad4038d05537793eed9999952ba1b34c6"},
 ]
 "screeninfo 0.8.1" = [
     {url = "https://files.pythonhosted.org/packages/6e/bf/c5205d480307bef660e56544b9e3d7ff687da776abb30c9cb3f330887570/screeninfo-0.8.1-py3-none-any.whl", hash = "sha256:e97d6b173856edcfa3bd282f81deb528188aff14b11ec3e195584e7641be733c"},
     {url = "https://files.pythonhosted.org/packages/ec/bb/e69e5e628d43f118e0af4fc063c20058faa8635c95a1296764acc8167e27/screeninfo-0.8.1.tar.gz", hash = "sha256:9983076bcc7e34402a1a9e4d7dabf3729411fd2abb3f3b4be7eba73519cd2ed1"},
 ]
+"setuptools 67.8.0" = [
+    {url = "https://files.pythonhosted.org/packages/03/20/630783571e76e5fa5f3e9f29398ca3ace377207b8196b54e0ffdf09f12c1/setuptools-67.8.0.tar.gz", hash = "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"},
+    {url = "https://files.pythonhosted.org/packages/f5/2c/074ab1c5be9c7d523d8d6d69d1f46f450fe7f11713147dc9e779aa4ca4ea/setuptools-67.8.0-py3-none-any.whl", hash = "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f"},
+]
 "six 1.12.0" = [
     {url = "https://files.pythonhosted.org/packages/73/fb/00a976f728d0d1fecfe898238ce23f502a721c0ac0ecfedb80e0d88c64e9/six-1.12.0-py2.py3-none-any.whl", hash = "sha256:3350809f0555b11f552448330d0b52d5f24c91a322ea4a15ef22629740f3761c"},
     {url = "https://files.pythonhosted.org/packages/dd/bf/4138e7bfb757de47d1f4b6994648ec67a51efe58fa907c1e11e350cddfca/six-1.12.0.tar.gz", hash = "sha256:d16a0141ec1a18405cd4ce8b4613101da75da0e9a7aec5bdd4fa804d0e0eba73"},
 ]
+"sklearn 0.0.post5" = [
+    {url = "https://files.pythonhosted.org/packages/7a/93/e0e1b1e98f39dfca7ec9795cb46f6e09e88a2fd5d4a28e4b3d1f618a2aec/sklearn-0.0.post5.tar.gz", hash = "sha256:7377c714a03a79bbe9196f435db931fd2a6fa8c68514da7ed3a251fd08c52e2c"},
+]
+"smart-open 6.3.0" = [
+    {url = "https://files.pythonhosted.org/packages/47/80/c2d1bdd36c6b64ae566d9a29724291510e4f3796ce99639d3c2999286284/smart_open-6.3.0-py3-none-any.whl", hash = "sha256:b4c9ae193ad6d3e7add50944b86afa0d150bd821ab8ec21edb26d9a06b66f6a8"},
+    {url = "https://files.pythonhosted.org/packages/b0/2b/ebc6d835bb354eb6d7f5f560be53dc746dab84d0958c363a082bfdf1e862/smart_open-6.3.0.tar.gz", hash = "sha256:d5238825fe9a9340645fac3d75b287c08fbb99fb2b422477de781c9f5f09e019"},
+]
 "sortedcontainers 2.4.0" = [
     {url = "https://files.pythonhosted.org/packages/32/46/9cb0e58b2deb7f82b84065f37f3bffeb12413f947f9388e4cac22c4621ce/sortedcontainers-2.4.0-py2.py3-none-any.whl", hash = "sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0"},
     {url = "https://files.pythonhosted.org/packages/e8/c4/ba2f8066cceb6f23394729afe52f3bf7adec04bf9ed2c820b39e19299111/sortedcontainers-2.4.0.tar.gz", hash = "sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88"},
 ]
 "soupsieve 2.4.1" = [
     {url = "https://files.pythonhosted.org/packages/47/9e/780779233a615777fbdf75a4dee2af7a345f4bf74b42d4a5f836800b9d91/soupsieve-2.4.1.tar.gz", hash = "sha256:89d12b2d5dfcd2c9e8c22326da9d9aa9cb3dfab0a83a024f05704076ee8d35ea"},
     {url = "https://files.pythonhosted.org/packages/49/37/673d6490efc51ec46d198c75903d99de59baffdd47aea3d071b80a9e4e89/soupsieve-2.4.1-py3-none-any.whl", hash = "sha256:1c1bfee6819544a3447586c889157365a27e10d88cde3ad3da0cf0ddf646feb8"},
 ]
+"spacy 3.5.3" = [
+    {url = "https://files.pythonhosted.org/packages/05/eb/a67f2bf174bb23844d007df56c0b393ff7e16f7d4909e83a394f79536aa4/spacy-3.5.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:77032fb9f1434ead183e5755e8b4edb58383577c9a14cdb784106aa9771126fc"},
+    {url = "https://files.pythonhosted.org/packages/0a/99/e5d68754b79d24e1ab0f8aa5271e16dfa019cae75c1ae6f8c75b10dff42c/spacy-3.5.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6ff8e6408d7672cdfd1b2035d2b5ca36b6c107c9b46debd9e5ba634700f761f5"},
+    {url = "https://files.pythonhosted.org/packages/13/fc/c7dc724bcfb63891929bd1079e525d10950d0d2131e886dec18b24e255b2/spacy-3.5.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c555e20187d7db210e3823eedff0f6fb029d23bc8e138342791f305510bf0c66"},
+    {url = "https://files.pythonhosted.org/packages/3b/ba/71bfe1dc76cefbf56833c2ee725fc56acb268f012170eb30082b7807cacd/spacy-3.5.3-cp37-cp37m-win_amd64.whl", hash = "sha256:13e54e45b447b6f52c7a050c69898fb7cab5dfc769dc073cc325b4ee8b278893"},
+    {url = "https://files.pythonhosted.org/packages/4c/a6/ea3bb98bb7fcb6177c3b44e778d17e3aaebfa283feb6763578abaa8664de/spacy-3.5.3.tar.gz", hash = "sha256:35971d6721576538d6c423c66a09ce00bf66e10e40726a57b7a81993180c248c"},
+    {url = "https://files.pythonhosted.org/packages/52/96/0d71f461848412a713d5ab25a0d5bf4e6160ca10fb52670f5c7dad3c5af0/spacy-3.5.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0b628bdeb6484eb4bfb1141d43013420d0356fc111033430292aea29b34b79e3"},
+    {url = "https://files.pythonhosted.org/packages/5c/48/eca527569df63cbf90695034fd86844cdb6a94d7398d8f5200afc8a984ab/spacy-3.5.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:d584ff7e6f0c044a5b17ceb6276ea65f054b157f31ce924318bf9b2c75fb8729"},
+    {url = "https://files.pythonhosted.org/packages/5c/e5/d42361d6328ee7010c5a11ac380ab71ea387164478f22c183b2ba29c3340/spacy-3.5.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:87caac0b18404a3cd43da1823914f7f54b60d640e36cc7240a8d05dff548be9e"},
+    {url = "https://files.pythonhosted.org/packages/5e/1c/de91feda7ed83236ee7aac9044bc6b8b1f60dfcac316f2e876e2832e5bb7/spacy-3.5.3-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0c83c11310f9dd3872659e7907ee44b128b850775f9765557f890d817362e1df"},
+    {url = "https://files.pythonhosted.org/packages/5e/8c/8ded4533e98f2e21cb04d6fbbe788bf9848dfba4d956e7c9870ad2e5d51f/spacy-3.5.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:87a5d0d87bc00b0b2c620bea3e8b226cd6913130a723dcaaa07b03e5d933ff59"},
+    {url = "https://files.pythonhosted.org/packages/5f/ce/7cf5e92da74600e256109cba3c6694512e044e8cd35623330b678a932df1/spacy-3.5.3-cp310-cp310-win_amd64.whl", hash = "sha256:2474f1a78557c5697529c48c5c9190f590ead21fbddf47cde757b399b807746c"},
+    {url = "https://files.pythonhosted.org/packages/63/d2/f356de9a8f7e2bec5521253ff0bdb739db39cee8304bc793125dad5f08da/spacy-3.5.3-cp39-cp39-win_amd64.whl", hash = "sha256:c28b1bfda0d5b0abba961c8679e21767493d48572c94d54acb4018d27f89f4e1"},
+    {url = "https://files.pythonhosted.org/packages/7d/2b/b7455e78bf4a5754f8eb7c42f65a2d263955cb9da4fcaa75d0b8c0359980/spacy-3.5.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:0ef98c2f5e36682a88b55ed841548e27bf8a400746c6bba406933f299ea873fc"},
+    {url = "https://files.pythonhosted.org/packages/81/74/0c4546354851cae3ea1357a52a4a05b2387a5ae3c0523e991325071a3461/spacy-3.5.3-cp38-cp38-win_amd64.whl", hash = "sha256:f58297c982823b19476a8efab302d269202af997c0b6500590ee55cd363428e8"},
+    {url = "https://files.pythonhosted.org/packages/89/32/cceff71eee6f56c01292c0b39b1a0a64aa6b8fef343d946364f246cf2ab5/spacy-3.5.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9f01ee5285a40d09c45c71bf756eb360de6ca4bb7d00aab4ca20e5379bb69bce"},
+    {url = "https://files.pythonhosted.org/packages/97/00/747b4dadfe56f8cffa24b9348a805be295d3dd969a8233acd294af0274d7/spacy-3.5.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a06285f19aaf1b4ea8d0c60285cd8712f9577a4cc64984e0841fa213a465e364"},
+    {url = "https://files.pythonhosted.org/packages/9c/5d/a838d749726712d7b04a35e7f11eb1e6ae0c9a1f6cf41e99f520bdb26a75/spacy-3.5.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d82d1aeae9e8ee04ccf863a42690493b0b0b912be81783bf737c5963e6e5a8c4"},
+    {url = "https://files.pythonhosted.org/packages/a1/23/39346123907c196fbf402e4a64b426cc32b0d6523b3208ee34b9c4385bf7/spacy-3.5.3-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9248ed4f4daa1e969dda69fe725b2085edbda10c562642d37212f2703971b4ca"},
+    {url = "https://files.pythonhosted.org/packages/a6/94/73c7b82b42aecd6097f154304a44b3d1a68ec819eb29d40898d70f8423f1/spacy-3.5.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:4eaa68b677b1292381bade13d5b20342e31791d3ffdaa261eca3c3c0687bf53f"},
+    {url = "https://files.pythonhosted.org/packages/ad/38/8a2307a1ba99c251c78d3f27574571ce4a34ef7a0778495c90f748379343/spacy-3.5.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:acc3ec415ba804515ff1449b13fefc07b393ea6a1ac3461b66b32f62b852467b"},
+    {url = "https://files.pythonhosted.org/packages/ad/7f/a7fe870035451cfa015703a75c90d8a90987ff0b5c6ad36ba7accb8380a7/spacy-3.5.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:59a473b8fbd79a22fdc98c017b14135b5c60c1813de01490a1eaa232a95a538b"},
+    {url = "https://files.pythonhosted.org/packages/c8/1c/ebfb91adee72b5c98f707ceaeeec9bc8d54346f5a7788dcae77c695bb53a/spacy-3.5.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:902f511ea8f8d9336d62b252f61d9068d93824ae70c5cb048954a3017cc38f1b"},
+    {url = "https://files.pythonhosted.org/packages/d0/51/5b8c366d90d1910e088e1cd5fbecea566d860beb056ec19d7a93f4604367/spacy-3.5.3-cp311-cp311-win_amd64.whl", hash = "sha256:3549364d4b2bf01736667e3fba3ce599e73ba281f003225de1033a648d5563f9"},
+    {url = "https://files.pythonhosted.org/packages/d3/ec/4911b58c65c5cb1c275deedbf0ebccdff417b9bded7741fcbf5944fd1603/spacy-3.5.3-cp36-cp36m-win_amd64.whl", hash = "sha256:98dc4240dd2e27ce33a63f796ed3baf1c1b474e85ade5083b6cb604021423bf1"},
+    {url = "https://files.pythonhosted.org/packages/db/24/799d2a80c0936775c001e223e4340e79a5795820cafafbd764a9755132ee/spacy-3.5.3-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fa543a185aabf8b33b7e280849fa4f1ae552a34e95a4b6a910d322527def7064"},
+    {url = "https://files.pythonhosted.org/packages/e0/eb/b3cdba6e38edc8acce5b58d1dd0e37f3954f36e036836735bce99f5afc8e/spacy-3.5.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a59cea275f5724494c77aec66b1758e42268504c34d055a6db2e95f652bd87a5"},
+    {url = "https://files.pythonhosted.org/packages/e9/5e/58270160d86c325d1932e83f3a46e7d112f97b5356669ef45bac311a8c26/spacy-3.5.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:860702748e654489e37464a5fca1444ee1b2534572084d416534a88646639c48"},
+    {url = "https://files.pythonhosted.org/packages/fb/79/bf46c571cee35037f4c37c79658e548d89cb804febcf39f6bb814e06a575/spacy-3.5.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9f5c4ca98f12e14f13dba08139c62671a623e6ff2d0d96783f8d09b33a8cd973"},
+]
+"spacy-legacy 3.0.12" = [
+    {url = "https://files.pythonhosted.org/packages/c3/55/12e842c70ff8828e34e543a2c7176dac4da006ca6901c9e8b43efab8bc6b/spacy_legacy-3.0.12-py2.py3-none-any.whl", hash = "sha256:476e3bd0d05f8c339ed60f40986c07387c0a71479245d6d0f4298dbd52cda55f"},
+    {url = "https://files.pythonhosted.org/packages/d9/79/91f9d7cc8db5642acad830dcc4b49ba65a7790152832c4eceb305e46d681/spacy-legacy-3.0.12.tar.gz", hash = "sha256:b37d6e0c9b6e1d7ca1cf5bc7152ab64a4c4671f59c85adaf7a3fcb870357a774"},
+]
+"spacy-loggers 1.0.4" = [
+    {url = "https://files.pythonhosted.org/packages/62/8c/814e0bd139a8c94b50298be3a4e640d90cdce78efe0099e373a767b7d854/spacy_loggers-1.0.4-py3-none-any.whl", hash = "sha256:e050bf2e63208b2f096b777e494971c962ad7c1dc997641c8f95c622550044ae"},
+    {url = "https://files.pythonhosted.org/packages/c5/ae/54d769684df039b55ecabab354b2bd3f8cbd9f75386ee6d2d65a54120328/spacy-loggers-1.0.4.tar.gz", hash = "sha256:e6f983bf71230091d5bb7b11bf64bd54415eca839108d5f83d9155d0ba93bf28"},
+]
 "speechrecognition 3.8.1" = [
     {url = "https://files.pythonhosted.org/packages/26/e1/7f5678cd94ec1234269d23756dbdaa4c8cfaed973412f88ae8adf7893a50/SpeechRecognition-3.8.1-py2.py3-none-any.whl", hash = "sha256:4d8f73a0c05ec70331c3bacaa89ecc06dfa8d9aba0899276664cda06ab597e8e"},
 ]
 "sqlite-fts4 1.0.3" = [
     {url = "https://files.pythonhosted.org/packages/51/29/0096e8b1811aaa78cfb296996f621f41120c21c2f5cd448ae1d54979d9fc/sqlite_fts4-1.0.3-py3-none-any.whl", hash = "sha256:0359edd8dea6fd73c848989e1e2b1f31a50fe5f9d7272299ff0e8dbaa62d035f"},
     {url = "https://files.pythonhosted.org/packages/c2/6d/9dad6c3b433ab8912ace969c66abd595f8e0a2ccccdb73602b1291dbda29/sqlite-fts4-1.0.3.tar.gz", hash = "sha256:78b05eeaf6680e9dbed8986bde011e9c086a06cb0c931b3cf7da94c214e8930c"},
 ]
-"sqlite-utils 3.31" = [
-    {url = "https://files.pythonhosted.org/packages/61/c9/99abf36fcef22959316cff00a7f07b413256ad97ab803ee45d6de78f2a52/sqlite_utils-3.31-py3-none-any.whl", hash = "sha256:95849cf62a9d6aa7df2dd27dfc615c0ee71c515516284a7d85e2c061021893c9"},
-    {url = "https://files.pythonhosted.org/packages/e8/da/6f34fd782e805f275ac17ecaba247db6c53eeaf340907c0e536366b6de1b/sqlite-utils-3.31.tar.gz", hash = "sha256:54989f3d09ed121f9df97831d041738ae48771d3ca85008946f1bc1884109a8a"},
+"sqlite-utils 3.32.1" = [
+    {url = "https://files.pythonhosted.org/packages/1a/95/b6fe852980c9494bf8a5e99d017cc6b864f9807a3e082c7837c267302217/sqlite-utils-3.32.1.tar.gz", hash = "sha256:6c28fe32fcebd658a1691dedfa4d111499ad302cc0139c5a5893a590d461848a"},
+    {url = "https://files.pythonhosted.org/packages/9e/eb/144eb61fd739b78d412d84d2d79148a4c5f3160c766317e9a19cd4ce3160/sqlite_utils-3.32.1-py3-none-any.whl", hash = "sha256:dfa124c4f752d67b2a36aa41929c51c699d81364b7b076218885a5ea714610d0"},
+]
+"srsly 2.4.6" = [
+    {url = "https://files.pythonhosted.org/packages/03/46/bfa8823b635ca9867c130d6a52506d132249293063a5cb0fee0358014d84/srsly-2.4.6-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:0522d9aeaf58c6d58ee0cec247653a460545422d3266b2d970df7af1530f3dcc"},
+    {url = "https://files.pythonhosted.org/packages/20/25/4dba38f470b4683b68ee741b85d852248074ce90eee503490a543c279c1f/srsly-2.4.6-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:99131465fea74aa5e80dbba6effad10ae661bee2c3fbc1fd6da8a1e954e031d0"},
+    {url = "https://files.pythonhosted.org/packages/29/19/c9af82aca65180b187f335bfbfa52719e2056367956ebbf32fcabff46b37/srsly-2.4.6-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2261ef76f6b8d4029b9d2fc4a65ac505a760d2ea1de0132fc4b423883f7df52e"},
+    {url = "https://files.pythonhosted.org/packages/29/ab/e819adf93bee080c594d3207cc96e0263f5094967246cfd6b09356093cd5/srsly-2.4.6-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:720715be0efb9646ab64850185ecd22fe6ace93027d02f6367bdc8842450b369"},
+    {url = "https://files.pythonhosted.org/packages/38/1c/66e7908dd223eb6e0befee2056ae1ccc64451a589380ea8e841ddbea976b/srsly-2.4.6-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:02b0708878f6a1e344284ae7c65b36a9ad8178eeff71583cd212d2d379f0e2ce"},
+    {url = "https://files.pythonhosted.org/packages/39/b0/79ce59ed8af4fac864899a873b679f5e5b1e2808179099473c9911133e95/srsly-2.4.6-cp36-cp36m-win_amd64.whl", hash = "sha256:bac2b2fa1f315c8a50e7807002a064e892be21c95735334f39d2ec104c00a8f0"},
+    {url = "https://files.pythonhosted.org/packages/5c/99/2e0c54aba2e8711852713c9b4ae8989fe9487816e58d21ab837ffb87e425/srsly-2.4.6-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0e5725f18a76971fc00e788a254bc2da6e119d69d491a811a6d387de77b72ca2"},
+    {url = "https://files.pythonhosted.org/packages/5e/39/d4f11f3b8dea2bc2783ddb23cd1dd56422d948fe08f3b900b97c7ab1aaea/srsly-2.4.6-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:9b96569976420be2ac3716db9ac05b06bf4cd7a358953879ba34f03c9533c123"},
+    {url = "https://files.pythonhosted.org/packages/75/18/7b25e88e7e7042d964554966838b36821ee7f95bddd397ce95e67d6ad5ba/srsly-2.4.6-cp38-cp38-win_amd64.whl", hash = "sha256:0ca1b1065edeca0cbc4a75ef15e915189bfd4b87c8256d542ec662168dd17627"},
+    {url = "https://files.pythonhosted.org/packages/7d/50/c5dcea9cba3f3d698a847bda584be85e414a4a5cdae8019c4a7f4434d377/srsly-2.4.6.tar.gz", hash = "sha256:47b41f323aba4c9c3311abf60e443c03a9efe9c69f65dc402d173c32f7744a6f"},
+    {url = "https://files.pythonhosted.org/packages/7e/5a/53eb6724aac9bdb75fd189531c5de053a19b4828208e52b29e09000d8347/srsly-2.4.6-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:da8d393ac59cba12b92c27c53550417200601d0f2a9aa50c1559cf5ce9cb9473"},
+    {url = "https://files.pythonhosted.org/packages/8a/fe/7d1e987bc119382cac80a19eaf39672ad36ede80fa6b2ba1b7a4f1546d86/srsly-2.4.6-cp37-cp37m-win_amd64.whl", hash = "sha256:f1fb1ca8e2415bfd9ce1e3d8612dbbd85dd06c574a0a96a0223265c382950b5a"},
+    {url = "https://files.pythonhosted.org/packages/9a/59/d5d6a3d1ad57e91a0bc305f7bf37da5b033c5e4c0cdcf9dcf47ff1c2e8a8/srsly-2.4.6-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1da8ac70f994644069451b4ab5fe5d2649218871409ab89f8421e79b0eace76b"},
+    {url = "https://files.pythonhosted.org/packages/aa/f3/1493eafd95cc74264a3fa89e5b83a93cfa0c5f63c17d63e60aa939d0aee6/srsly-2.4.6-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:73acd407c66fa943bbaa8d473c30ea548b31ba4079b51483eda65df94910b61f"},
+    {url = "https://files.pythonhosted.org/packages/b0/62/95a72536387ce81c543c2ab970d1d6d7c8af07a35c7e7feb7080407350b2/srsly-2.4.6-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9fb1426313af7c560c728fbe8c3cc8e7cc443f5aa489b04a26adc73645214b91"},
+    {url = "https://files.pythonhosted.org/packages/b2/03/5890066e070e5be5b8653833b10743c2ff9345fcc7e88bf029e683c60fbc/srsly-2.4.6-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e5c5074628249385640f4fe4ac237fd93631a023938476ea258139d12abb17f9"},
+    {url = "https://files.pythonhosted.org/packages/c3/8b/f318de2db4826429da431152758336415451553e5d8e96949bfcbfc87dbe/srsly-2.4.6-cp311-cp311-win_amd64.whl", hash = "sha256:73ce7c532fecbd8d7ab946fd2b5fa1d767d554526e330e55d7704bcf522c9f66"},
+    {url = "https://files.pythonhosted.org/packages/c4/f7/046904fc285878fd8ce24c63bdf923ad090ed85257d98404d121086a1593/srsly-2.4.6-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:52e3a0a760fb7723c74e566d0c064da78e5707d65d8f69b1d3c2e05b72e3efb2"},
+    {url = "https://files.pythonhosted.org/packages/c7/5f/28b5d51a7da971996cdbc7fec3c740a3c118eb92088eeb84ff687d1fc461/srsly-2.4.6-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:3a6811eb797101b549fece201c03ba794ed731e9e2d58b81ea56eb3219ed2c8e"},
+    {url = "https://files.pythonhosted.org/packages/cc/35/a2e428b625014c582c5ce95766be40da9fd53b82f3b6e8b4a22a91b96241/srsly-2.4.6-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:03477c648b76571a5ab0723423fc03ada74e747c4354357feef92c098853246f"},
+    {url = "https://files.pythonhosted.org/packages/d5/dc/827c78adf0f0c9c006645877a70bc4c7a4f62a150253053e6bd70b2031a8/srsly-2.4.6-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e4a0152f766930aa41f45bf571b7f6e99206a02810d964cc7bcbd81685e3b624"},
+    {url = "https://files.pythonhosted.org/packages/db/a3/ea3c623d60c8be5ba11e43e9dfc270518107691f91dd5052322a5bc44d85/srsly-2.4.6-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:5a9833c0a870e17c67a9452ed107b3ec033fa5b7addead51af5977fdafd32452"},
+    {url = "https://files.pythonhosted.org/packages/e1/48/16e70c08707949914f3ceaad78be077b64db62217fa80f1247d13ed18f47/srsly-2.4.6-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:12b9e6d5a87c64e1d4a4a43fd6c94f98b5c48076c569804072e5fe45f1703c32"},
+    {url = "https://files.pythonhosted.org/packages/e8/91/5acb03c643967d3117b6cb4a103b17b6a2c4828a1d0a1f1c3117a103759d/srsly-2.4.6-cp310-cp310-win_amd64.whl", hash = "sha256:02ab79c59e4b0eba4ba44d64b4aeccb5df1379270f3970dc7e30f1eef6cd3851"},
+    {url = "https://files.pythonhosted.org/packages/ec/91/9e43d4440ae8ee1cd9414a8eeae2e30f16afde3b4ea988570497841faca0/srsly-2.4.6-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0355d57e89382bc0852d30b000f1d04f0bf1da2a739f60f0427a00b6ea1cd146"},
+    {url = "https://files.pythonhosted.org/packages/f0/81/6baa09ed1f74dd217b0242ba64affbcab61b59903af6b94ca4340887833d/srsly-2.4.6-cp39-cp39-win_amd64.whl", hash = "sha256:52a3b4d2949d9b7623b459054526bc3df04cbd9a8243c4786f13e3c956faf251"},
+    {url = "https://files.pythonhosted.org/packages/f2/58/f248173c08d0ce8347e1cc970f4748ca88dcdfcf9c8fb8c27495d67a703e/srsly-2.4.6-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7dc1c3877618d67a44ec74830510cd72d54fcfb32339388f2c6cbd559d27d20e"},
+    {url = "https://files.pythonhosted.org/packages/fc/87/b2d7f5e8b3dd366294e29b7e010738c1c0d01da665546f20f788ce91ecef/srsly-2.4.6-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9742e5f4205c5484cea925ff24b1bd850f1e9291bd0ada6dfe1ec2b715e732b5"},
 ]
 "ssort 0.11.6" = [
     {url = "https://files.pythonhosted.org/packages/27/c6/4fdb102b282380d5b4791d90302ba8778689f24bef118707fd50f037752e/ssort-0.11.6.tar.gz", hash = "sha256:21fec493487f32dff50d30efa5b6aad18286e9817600b64bfe686ae062bae7ae"},
 ]
 "stack-data 0.6.2" = [
     {url = "https://files.pythonhosted.org/packages/6a/81/aa96c25c27f78cdc444fec27d80f4c05194c591465e491a1358d8a035bc1/stack_data-0.6.2-py3-none-any.whl", hash = "sha256:cbb2a53eb64e5785878201a97ed7c7b94883f48b87bfb0bbe8b623c74679e4a8"},
     {url = "https://files.pythonhosted.org/packages/db/18/aa7f2b111aeba2cd83503254d9133a912d7f61f459a0c8561858f0d72a56/stack_data-0.6.2.tar.gz", hash = "sha256:32d2dd0376772d01b6cb9fc996f3c8b57a357089dec328ed4b6553d037eaf815"},
@@ -2629,28 +3064,66 @@
     {url = "https://files.pythonhosted.org/packages/40/44/4a5f08c96eb108af5cb50b41f76142f0afa346dfa99d5296fe7202a11854/tabulate-0.9.0-py3-none-any.whl", hash = "sha256:024ca478df22e9340661486f85298cff5f6dcdba14f3813e8830015b9ed1948f"},
     {url = "https://files.pythonhosted.org/packages/ec/fe/802052aecb21e3797b8f7902564ab6ea0d60ff8ca23952079064155d1ae1/tabulate-0.9.0.tar.gz", hash = "sha256:0095b12bf5966de529c0feb1fa08671671b3368eec77d7ef7ab114be2c068b3c"},
 ]
 "textract 1.6.5" = [
     {url = "https://files.pythonhosted.org/packages/6b/3e/ac16b6bf28edf78296aea7d0cb416b49ed30282ac8c711662541015ee6f3/textract-1.6.5-py3-none-any.whl", hash = "sha256:0accd78ec42864e3e3827f9ef798ced9aac4727b664303b724a198fed73fa438"},
     {url = "https://files.pythonhosted.org/packages/81/9f/dd29fcec368f007d44e51f0273489d5172a6d32ed9c796df5054fbb31c9f/textract-1.6.5.tar.gz", hash = "sha256:68f0f09056885821e6c43d8538987518daa94057c306679f2857cc5ee66ad850"},
 ]
+"thinc 8.1.10" = [
+    {url = "https://files.pythonhosted.org/packages/05/d4/e0f3abbccbcf9961fae42d8ec2ed65abdd582aa9589208a59a37fb061a7d/thinc-8.1.10-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a5af0392bdc63c621ba1def80ec98d753be9a27ebe1cf812bed2760371f20456"},
+    {url = "https://files.pythonhosted.org/packages/0d/0a/7bca8c34b725819d5e4d4eec2e24a696f6ff9282b68f7d24a7a151b1c2bd/thinc-8.1.10-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d9bee276fb1f820b9a5f80c08655eb78dc2f368f3c22fd33e958e0fedeaac09b"},
+    {url = "https://files.pythonhosted.org/packages/11/a5/af6e43bf9be5bf1086e5129466273c2582faf81689b3609caad880780a5f/thinc-8.1.10-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5fd1aa467f445860ae8f0943ab80e41be9b64243522c165bea452ad39d4ff46f"},
+    {url = "https://files.pythonhosted.org/packages/15/c4/5d0a9b7d7627f54d855e31bba56535e664be0131f0b9397e1f7627a01b7e/thinc-8.1.10-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:0bf181b47d88c60a961e0cd05eec1143d949dd8e7e3523e13f4e8f1ea32f0004"},
+    {url = "https://files.pythonhosted.org/packages/1c/2b/66e103eefdf1deea66299267aa738c61ee40d8c818c712bcec39af25b57c/thinc-8.1.10-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:0bdf3f4e4a2fc0a4c5887e9114340ddb60ccc7b85f2cf92affdc68da82430575"},
+    {url = "https://files.pythonhosted.org/packages/1f/bb/ad504f0ea3dd158bd9423430fa56d68fa0891947f9dbb4a21296f936990e/thinc-8.1.10-cp37-cp37m-win_amd64.whl", hash = "sha256:d63fa0bd3e60931c76617e993042deef875f57b1679354ac2f0072e621e106d1"},
+    {url = "https://files.pythonhosted.org/packages/30/23/0ec4a96a5c0c39246233946be12144d651e5d99b0a4dee812b05a5c9f4be/thinc-8.1.10-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b432bf27e4724e2f470e5f36455530906d86a81505a3b406f2f4f5b4644f77d8"},
+    {url = "https://files.pythonhosted.org/packages/42/4c/dc0535299b86b301c606496fd341c6692136cb8fda93f0a0684abe2f123f/thinc-8.1.10-cp38-cp38-win_amd64.whl", hash = "sha256:21a41c90122e9b8a6b33d5ba05913fd8a763757a2b49e0243eed0bce7722d661"},
+    {url = "https://files.pythonhosted.org/packages/55/25/8563397bf5216c6afee7cf603694094e8f4b0b151c6645504030363d63be/thinc-8.1.10-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:83da33e05fda126e85e385aaeb2eb8d1ae19368c5bc67f23b88bc2927738b5cf"},
+    {url = "https://files.pythonhosted.org/packages/5a/62/ab663818cb333eae796622503ce0a41cbb5ef49a34559f26171d589032ee/thinc-8.1.10-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a65a1e824711b30e0c35ebfb833681b64c6cb2762364548a210c3740838b9d91"},
+    {url = "https://files.pythonhosted.org/packages/62/77/f714e95bf30e8f540bcb9bdf0c5e88358b894d45be0333151750590bb94c/thinc-8.1.10-cp311-cp311-win_amd64.whl", hash = "sha256:108dcfef6ad1bef46d00ad31edc5fd3ab4d36c0cadb92cfbdb2f92d060acd8a0"},
+    {url = "https://files.pythonhosted.org/packages/6b/6d/925ed638b71d51e68709cf8931cfb2f10cc5bc9d9fafcaa9ac7946cc76f5/thinc-8.1.10-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5c9cf2c9d8e44e1edeffe878cb137cbfe5ae1540621b5878be8e5e8d4924d757"},
+    {url = "https://files.pythonhosted.org/packages/6e/42/057893864c5b981c6b1206701bdd1a38ec5d586e0e77fde5be239348d7a0/thinc-8.1.10-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:18380a440d617fa704daa5018ed5e7d5a50efd9c237ad536a84047be3bcb767c"},
+    {url = "https://files.pythonhosted.org/packages/77/f3/c16f1a6aa534fa5c70932b47bf5e87e1e1ea21b9e74f73903a47bc612c02/thinc-8.1.10-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:042be0f014d896b826d8c0891b7bc8772464a91661938c61cdd7296cef19280d"},
+    {url = "https://files.pythonhosted.org/packages/7a/00/c1458347892353d790387819b4cac7f3014db9a558b58ef68f55fbb0c64d/thinc-8.1.10-cp39-cp39-win_amd64.whl", hash = "sha256:c245e6a5fcb71fcf23cb329f296349a4925b176fad5713571bb4f0fc8787ad7c"},
+    {url = "https://files.pythonhosted.org/packages/8b/68/e2fc0f826342380eb990955b1483c3abbcf2651fa9a9501fbbd952f97e2b/thinc-8.1.10-cp310-cp310-win_amd64.whl", hash = "sha256:e5b2232e737c25fef3116597d1458fef38ddb7237649747686ce4d4531bb84a3"},
+    {url = "https://files.pythonhosted.org/packages/8f/26/a369896061f1436b6015ba4047652e2e7eb99fdf54d705098dbbfdd0dec6/thinc-8.1.10-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:524e6eb2436084968db1a713cfb5ea99b1b2e3363330d4aac8a403487a16d7c2"},
+    {url = "https://files.pythonhosted.org/packages/91/77/377c6d2b4beb67b653d58dc37737016c68af53ffab32a2eaba49a1a04c85/thinc-8.1.10-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:ee75162bfb8aab24bd59604c01935abe1602bbd478064a4a6199d3506cb57679"},
+    {url = "https://files.pythonhosted.org/packages/99/cd/b3418cbba056b01211fc8c4a8718445937fcfcd5b9d8bc350b2a84579bc8/thinc-8.1.10-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:715ed60ddf1ddf5f98b454b2495fddbbfdb947d77bd47a241d1981d3f58ac9a0"},
+    {url = "https://files.pythonhosted.org/packages/9a/88/8723d77af69ca490a481d72e7eb526e4edf9d06b0f15872698057378a140/thinc-8.1.10-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2d08eb7c15592d4212cd729d782b8be1daa2ed5248a8169991c4f63659bc6266"},
+    {url = "https://files.pythonhosted.org/packages/a2/8a/7a5500519eb4c3162612c01a8aa6ce18d729b161835a836b1b385ea9c9f1/thinc-8.1.10-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ea3da2c0fb9012b6bff8b43d86dc34fd2db463f5b5e5fa725e2f5c49d29620b5"},
+    {url = "https://files.pythonhosted.org/packages/a4/1e/55884d1e156a5921e161bbaada7d948c9749249852b2a526446f2e788908/thinc-8.1.10-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:50271826c3737168cd9409620c9fcd3f6315136d2fff08279c213a21a5c438e8"},
+    {url = "https://files.pythonhosted.org/packages/a6/0b/fafa1853bf5db8403a1ff2499b9a6b811b7d4228fc044a1f03345017cf4c/thinc-8.1.10-cp36-cp36m-win_amd64.whl", hash = "sha256:bc321d0fbb8e146de4c152d36ea6000de0669fe081fd9777c8768ad9b4478839"},
+    {url = "https://files.pythonhosted.org/packages/b0/c3/c3f124964f216e728acb7205f41609f9799177f13380298adf1ecfd7d8f7/thinc-8.1.10-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:575b7dbe3a5d773c12f5dd6e366d942ad3c3ef7a5381332ba842bdbaf4d3e820"},
+    {url = "https://files.pythonhosted.org/packages/ba/dd/174a128d0e84814b0f05ec5de9ecf65e3a9b3c4882823610736385df21ab/thinc-8.1.10-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:dbd1dc4394352d80af22131e1a238238eded59de19b55f77e6237436f4865b2c"},
+    {url = "https://files.pythonhosted.org/packages/d3/60/c82a50fdde18d4544719c88d8e8adc0ba9ea23bb444b03e7296982f93a58/thinc-8.1.10-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:bd9b678bcbf3f3a21260b2f55a65742aeeb7f5442c3ceb475378d95e0e99dc44"},
+    {url = "https://files.pythonhosted.org/packages/f3/5c/4e8671aa258dbefce508aa0236fae572bf7bbd9784fad3637d76a858ff6f/thinc-8.1.10-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d31f6834f1b1c428718a9668b7a06b74854a9217ba1d8186b41e48146d487fa3"},
+    {url = "https://files.pythonhosted.org/packages/fb/aa/daaff7c5c5878cad416b906bb8b573b5a4023e11a138ad082f1fb089eab8/thinc-8.1.10.tar.gz", hash = "sha256:6c4a48d7da07e044e84a68cbb9b22f32f8490995a2bab0bfc60e412d14afb991"},
+]
 "tinytag 1.9.0" = [
     {url = "https://files.pythonhosted.org/packages/33/58/ff5f7a345b6448b6ad3cb8dd3c9a6cb4100e3359468e5f984aaca2634213/tinytag-1.9.0.tar.gz", hash = "sha256:f8d71110e1e680a33d99202e00a5a698481d25d20173b81ba3e863423979e014"},
 ]
 "tomli 2.0.1" = [
     {url = "https://files.pythonhosted.org/packages/97/75/10a9ebee3fd790d20926a90a2547f0bf78f371b2f13aa822c759680ca7b9/tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {url = "https://files.pythonhosted.org/packages/c0/3f/d7af728f075fb08564c5949a9c95e44352e23dee646869fa104a3b2060a3/tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
+"tqdm 4.65.0" = [
+    {url = "https://files.pythonhosted.org/packages/3d/78/81191f56abb7d3d56963337dbdff6aa4f55805c8afd8bad64b0a34199e9b/tqdm-4.65.0.tar.gz", hash = "sha256:1871fb68a86b8fb3b59ca4cdd3dcccbc7e6d613eeed31f4c332531977b89beb5"},
+    {url = "https://files.pythonhosted.org/packages/e6/02/a2cff6306177ae6bc73bc0665065de51dfb3b9db7373e122e2735faf0d97/tqdm-4.65.0-py3-none-any.whl", hash = "sha256:c4f53a17fe37e132815abceec022631be8ffe1b9381c2e6e30aa70edc99e9671"},
+]
 "traitlets 5.9.0" = [
     {url = "https://files.pythonhosted.org/packages/39/c3/205e88f02959712b62008502952707313640369144a7fded4cbc61f48321/traitlets-5.9.0.tar.gz", hash = "sha256:f6cde21a9c68cf756af02035f72d5a723bf607e862e7be33ece505abf4a3bad9"},
     {url = "https://files.pythonhosted.org/packages/77/75/c28e9ef7abec2b7e9ff35aea3e0be6c1aceaf7873c26c95ae1f0d594de71/traitlets-5.9.0-py3-none-any.whl", hash = "sha256:9e6ec080259b9a5940c797d58b613b5e31441c2257b87c2e795c5228ae80d2d8"},
 ]
-"typing-extensions 4.5.0" = [
-    {url = "https://files.pythonhosted.org/packages/31/25/5abcd82372d3d4a3932e1fa8c3dbf9efac10cc7c0d16e78467460571b404/typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
-    {url = "https://files.pythonhosted.org/packages/d3/20/06270dac7316220643c32ae61694e451c98f8caf4c8eab3aa80a2bedf0df/typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
+"typer 0.7.0" = [
+    {url = "https://files.pythonhosted.org/packages/0d/44/56c3f48d2bb83d76f5c970aef8e2c3ebd6a832f09e3621c5395371fe6999/typer-0.7.0-py3-none-any.whl", hash = "sha256:b5e704f4e48ec263de1c0b3a2387cd405a13767d2f907f44c1a08cbad96f606d"},
+    {url = "https://files.pythonhosted.org/packages/e1/45/bcbc581f87c8d8f2a56b513eb994d07ea4546322818d95dc6a3caf2c928b/typer-0.7.0.tar.gz", hash = "sha256:ff797846578a9f2a201b53442aedeb543319466870fbe1c701eab66dd7681165"},
+]
+"typing-extensions 4.6.2" = [
+    {url = "https://files.pythonhosted.org/packages/38/60/300ad6f93adca578bf05d5f6cd1d854b7d140bebe2f9829561aa9977d9f3/typing_extensions-4.6.2-py3-none-any.whl", hash = "sha256:3a8b36f13dd5fdc5d1b16fe317f5668545de77fa0b8e02006381fd49d731ab98"},
+    {url = "https://files.pythonhosted.org/packages/be/fc/3d12393d634fcb31d5f4231c28feaf4ead225124ba08021046317d5f450d/typing_extensions-4.6.2.tar.gz", hash = "sha256:06006244c70ac8ee83fa8282cb188f697b8db25bc8b4df07be1873c43897060c"},
 ]
 "tzdata 2023.3" = [
     {url = "https://files.pythonhosted.org/packages/70/e5/81f99b9fced59624562ab62a33df639a11b26c582be78864b339dafa420d/tzdata-2023.3.tar.gz", hash = "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a"},
     {url = "https://files.pythonhosted.org/packages/d5/fb/a79efcab32b8a1f1ddca7f35109a50e4a80d42ac1c9187ab46522b2407d7/tzdata-2023.3-py2.py3-none-any.whl", hash = "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"},
 ]
 "tzlocal 5.0.1" = [
     {url = "https://files.pythonhosted.org/packages/84/d2/730a87f0dbf184760394a85088d0d2366a5a8a32bc32ffd869a83f1de854/tzlocal-5.0.1-py3-none-any.whl", hash = "sha256:f3596e180296aaf2dbd97d124fe76ae3a0e3d32b258447de7b939b3fd4be992f"},
@@ -2660,21 +3133,25 @@
     {url = "https://files.pythonhosted.org/packages/0c/ba/8dd7fa5f0b1c6a8ac62f8f57f7e794160c1f86f31c6d0fb00f582372a3e4/update_checker-0.18.0-py3-none-any.whl", hash = "sha256:cbba64760a36fe2640d80d85306e8fe82b6816659190993b7bdabadee4d4bbfd"},
     {url = "https://files.pythonhosted.org/packages/5c/0b/1bec4a6cc60d33ce93d11a7bcf1aeffc7ad0aa114986073411be31395c6f/update_checker-0.18.0.tar.gz", hash = "sha256:6a2d45bb4ac585884a6b03f9eade9161cedd9e8111545141e9aa9058932acb13"},
 ]
 "urllib3 1.25.11" = [
     {url = "https://files.pythonhosted.org/packages/56/aa/4ef5aa67a9a62505db124a5cb5262332d1d4153462eb8fd89c9fa41e5d92/urllib3-1.25.11-py2.py3-none-any.whl", hash = "sha256:f5321fbe4bf3fefa0efd0bfe7fb14e90909eb62a48ccda331726b4319897dd5e"},
     {url = "https://files.pythonhosted.org/packages/76/d9/bbbafc76b18da706451fa91bc2ebe21c0daf8868ef3c30b869ac7cb7f01d/urllib3-1.25.11.tar.gz", hash = "sha256:8d7eaa5a82a1cac232164990f04874c594c9453ec55eef02eab885aa02fc17a2"},
 ]
+"wasabi 1.1.1" = [
+    {url = "https://files.pythonhosted.org/packages/58/5f/1f2833d59abf53e24dbadc21b0565fe10c64545da8705faed8eff3b14745/wasabi-1.1.1-py3-none-any.whl", hash = "sha256:32e44649d99a64e08e40c1c96cddb69fad460bd0cc33802a53cab6714dfb73f8"},
+    {url = "https://files.pythonhosted.org/packages/8d/d3/abe7d7d745657e43af711bdc58d4c9016f63546795ec9b5b62b2d9b89fa6/wasabi-1.1.1.tar.gz", hash = "sha256:f5ee7c609027811bd16e620f2fd7a7319466005848e41b051a62053ab8fd70d6"},
+]
 "wcwidth 0.2.6" = [
     {url = "https://files.pythonhosted.org/packages/20/f4/c0584a25144ce20bfcf1aecd041768b8c762c1eb0aa77502a3f0baa83f11/wcwidth-0.2.6-py2.py3-none-any.whl", hash = "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e"},
     {url = "https://files.pythonhosted.org/packages/5e/5f/1e4bd82a9cc1f17b2c2361a2d876d4c38973a997003ba5eb400e8a932b6c/wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
-"websocket-client 1.5.1" = [
-    {url = "https://files.pythonhosted.org/packages/6d/9a/6c793729c9d48fcca155ce55e4dfafacffb7fb52a62e3ae2198846c31af6/websocket_client-1.5.1-py3-none-any.whl", hash = "sha256:cdf5877568b7e83aa7cf2244ab56a3213de587bbe0ce9d8b9600fc77b455d89e"},
-    {url = "https://files.pythonhosted.org/packages/8b/94/696484b0c13234c91b316bc3d82d432f9b589a9ef09d016875a31c670b76/websocket-client-1.5.1.tar.gz", hash = "sha256:3f09e6d8230892547132177f575a4e3e73cfdf06526e20cc02aa1c3b47184d40"},
+"websocket-client 1.5.2" = [
+    {url = "https://files.pythonhosted.org/packages/3f/f2/2624e12ef854ee667d92ac5dc7815932095e0852e5ff2b2bf57feda8a11b/websocket-client-1.5.2.tar.gz", hash = "sha256:c7d67c13b928645f259d9b847ab5b57fd2d127213ca41ebd880de1f553b7c23b"},
+    {url = "https://files.pythonhosted.org/packages/86/5c/2ebfbb7d4dbb7f35a1f70c40d003f7844d78945ac7c69757067ebaea9c78/websocket_client-1.5.2-py3-none-any.whl", hash = "sha256:f8c64e28cd700e7ba1f04350d66422b6833b82a796b525a51e740b8cc8dab4b1"},
 ]
 "websockets 11.0.3" = [
     {url = "https://files.pythonhosted.org/packages/03/28/3a51ffcf51ac45746639f83128908bbb1cd212aa631e42d15a7acebce5cb/websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e052b8467dd07d4943936009f46ae5ce7b908ddcac3fda581656b1b19c083d9b"},
     {url = "https://files.pythonhosted.org/packages/0a/84/68b848a373493b58615d6c10e9e8ccbaadfd540f84905421739a807704f8/websockets-11.0.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aa5003845cdd21ac0dc6c9bf661c5beddd01116f6eb9eb3c8e272353d45b3288"},
     {url = "https://files.pythonhosted.org/packages/0f/d8/a997d3546aef9cc995a1126f7d7ade96c0e16c1a0efb9d2d430aee57c925/websockets-11.0.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:619d9f06372b3a42bc29d0cd0354c9bb9fb39c2cbc1a9c5025b4538738dbffaf"},
     {url = "https://files.pythonhosted.org/packages/14/fc/5cbbf439c925e1e184a0392ec477a30cee2fabc0e63807c1d4b6d570fb52/websockets-11.0.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:b30c6590146e53149f04e85a6e4fcae068df4289e31e4aee1fdf56a0dead8f97"},
     {url = "https://files.pythonhosted.org/packages/16/49/ae616bd221efba84a3d78737b417f704af1ffa36f40dcaba5eb954dd4753/websockets-11.0.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e848f46a58b9fcf3d06061d17be388caf70ea5b8cc3466251963c8345e13f7eb"},
@@ -2752,17 +3229,17 @@
     {url = "https://files.pythonhosted.org/packages/61/86/cc8d1ff2ca31a312a25a708c891cf9facbad4eae493b3872638db6785eb5/wheel-0.40.0-py3-none-any.whl", hash = "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"},
     {url = "https://files.pythonhosted.org/packages/fc/ef/0335f7217dd1e8096a9e8383e1d472aa14717878ffe07c4772e68b6e8735/wheel-0.40.0.tar.gz", hash = "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873"},
 ]
 "xlrd 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/aa/05/ec9d4fcbbb74bbf4da9f622b3b61aec541e4eccf31d3c60c5422ec027ce2/xlrd-1.2.0.tar.gz", hash = "sha256:546eb36cee8db40c3eaa46c351e67ffee6eeb5fa2650b71bc4c758a29a1b29b2"},
     {url = "https://files.pythonhosted.org/packages/b0/16/63576a1a001752e34bf8ea62e367997530dc553b689356b9879339cf45a4/xlrd-1.2.0-py2.py3-none-any.whl", hash = "sha256:e551fb498759fa3a5384a94ccd4c3c02eb7c00ea424426e212ac0c57be9dfbde"},
 ]
-"xlsxwriter 3.1.0" = [
-    {url = "https://files.pythonhosted.org/packages/17/00/b99c915fa2118b9a1dd061a5bf82094c843ab481c714c6d826668df834ad/XlsxWriter-3.1.0.tar.gz", hash = "sha256:02913b50b74c00f165933d5da3e3a02cab4204cb4932722a1b342c5c71034122"},
-    {url = "https://files.pythonhosted.org/packages/bd/00/28d48d105fa914b460e9721b315af096937e2e82bf540932c68420ccd9e1/XlsxWriter-3.1.0-py3-none-any.whl", hash = "sha256:b70a147d36235d1ee835cfd037396f789db1f76740a0e5c917d54137169341de"},
+"xlsxwriter 3.1.2" = [
+    {url = "https://files.pythonhosted.org/packages/04/d4/3cc6a3cd112a91d95f554ca8909c8528addf06d79c51ccd40e39a6ff48e1/XlsxWriter-3.1.2.tar.gz", hash = "sha256:78751099a770273f1c98b8d6643351f68f98ae8e6acf9d09d37dc6798f8cd3de"},
+    {url = "https://files.pythonhosted.org/packages/37/94/25d3ec8587974de7ebd790232aa3155abfe44ed23df7ccaa4645977a1cbe/XlsxWriter-3.1.2-py3-none-any.whl", hash = "sha256:331508ff39d610ecdaf979e458840bc1eab6e6a02cfd5d08f044f0f73636236f"},
 ]
 "yarl 1.9.2" = [
     {url = "https://files.pythonhosted.org/packages/0e/b1/a65fcf0363ae8c08c0e586772a34cc15b4200bae163eed24258cc95cda90/yarl-1.9.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:566185e8ebc0898b11f8026447eacd02e46226716229cea8db37496c8cdd26e0"},
     {url = "https://files.pythonhosted.org/packages/10/b1/13887c4fbf885d64f4b8c1bac403338f7c1c07a34e63d767af8d0972c28d/yarl-1.9.2-cp37-cp37m-win32.whl", hash = "sha256:f364d3480bffd3aa566e886587eaca7c8c04d74f6e8933f3f2c996b7f09bee1b"},
     {url = "https://files.pythonhosted.org/packages/11/3d/785761e64dc90fda6feb9bd0459dc55ebe282a7d4564642a4a8ee277e0c0/yarl-1.9.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a74dcbfe780e62f4b5a062714576f16c2f3493a0394e555ab141bf0d746bb955"},
     {url = "https://files.pythonhosted.org/packages/12/27/efe7476bdadb2564d7775e0895df56f3e3adf39495094750fb319599180e/yarl-1.9.2-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:13414591ff516e04fcdee8dc051c13fd3db13b673c7a4cb1350e6b2ad9639ad3"},
     {url = "https://files.pythonhosted.org/packages/12/c0/18265b85980450b75641a32dd12635485241e295310c1b04e04ac0cc634e/yarl-1.9.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:38a3928ae37558bc1b559f67410df446d1fbfa87318b124bf5032c31e3447b74"},
@@ -2836,49 +3313,49 @@
     {url = "https://files.pythonhosted.org/packages/fb/2d/060ab740f64ea6ea2088e375c3046839faaf4bbba2b65a5364668bd765e7/yarl-1.9.2-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:84e0b1599334b1e1478db01b756e55937d4614f8654311eb26012091be109d59"},
     {url = "https://files.pythonhosted.org/packages/fe/7d/9d85f658b6f7c041ca3ba371d133040c4dc41eb922aef0a6ba917291d187/yarl-1.9.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aff634b15beff8902d1f918012fc2a42e0dbae6f469fce134c8a0dc51ca423bb"},
 ]
 "yt-dlp 2023.3.4" = [
     {url = "https://files.pythonhosted.org/packages/a7/df/498c57f641e9993376cf52489047158e6d660e8bab06b72c470ad5cce2bd/yt_dlp-2023.3.4-py2.py3-none-any.whl", hash = "sha256:40ca421407ce07c8fd700854fd978d58526ec6fff3468caa34ff1c7333b8dc34"},
     {url = "https://files.pythonhosted.org/packages/e8/4a/1e01f24fcb49191626e2b17d00e13a093315d03a9da09fccb1c75913e420/yt-dlp-2023.3.4.tar.gz", hash = "sha256:265d5da97a76c15d7d9a4088a67b78acd5dcf6f8cfd8257c52f581ff996ff515"},
 ]
-"zeroconf 0.62.0" = [
-    {url = "https://files.pythonhosted.org/packages/0d/e0/60524d75a31ec0bff0ae1c98caa89a0208a3bdcbc42214f3a3ead973d839/zeroconf-0.62.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4abd599668c0f03623df96b63afe8423f48c33296571d93610a2cf2f8bdf4a3f"},
-    {url = "https://files.pythonhosted.org/packages/11/c3/baedd0ca334879b82a57cae47ccb1fcef734cfd2e7bf2b9f8e8a9ede9928/zeroconf-0.62.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:64d34d01f215843cfa043aa3ad93da4bf16055c245fd254281c35c82dae6eb06"},
-    {url = "https://files.pythonhosted.org/packages/15/40/2cb92f4410243de98b1acbb045b42f634b7dbddc62adb737c98407a50846/zeroconf-0.62.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:b5efbf2d1bf5faed732d8ea8fc50001ca782c5f0292ca59d8e00a5777bf635e4"},
-    {url = "https://files.pythonhosted.org/packages/21/0b/7affc8fd467d9a583e47483708cf376c3812726421f4bbf0263ebdc05cc8/zeroconf-0.62.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:40021028da67058c5749c8388617f1ced3b57f8ec22c1a39dc7b44b7017a696b"},
-    {url = "https://files.pythonhosted.org/packages/28/1e/0da71cbb9d5e411ac4ad11750b5d6834ea5f0779bd532716f1f47ca4e976/zeroconf-0.62.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:499da0534ef3ea728fc02104386c87d178d6e0ad0727edcff619d29767e4e903"},
-    {url = "https://files.pythonhosted.org/packages/2f/c3/3c3fec9aeaa2b85584a319eb76321d3dc769c9185df96fafff7791e233dd/zeroconf-0.62.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:08c95a60c1fe967ce7bf722b908cdfc646fe9ba55952a67a3cb3dfcdf3cf5b37"},
-    {url = "https://files.pythonhosted.org/packages/40/55/44116a2e53ca357f9679f946bc2f1c1e13644482541db8b0f4a6ba9fde51/zeroconf-0.62.0-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:11a9172ebc5a768bdc4b09684814f8c2da8664d612ecbc0f63ebcb1092ca4624"},
-    {url = "https://files.pythonhosted.org/packages/41/06/040865a66caa75cf87bd8ca26e852ccd6c765b4d12231934e2af36d5da9b/zeroconf-0.62.0-pp37-pypy37_pp73-macosx_11_0_x86_64.whl", hash = "sha256:d44d7d1ad67e65f09a5384d88e2c6b783c533290374094b6bf314b8963f3f13d"},
-    {url = "https://files.pythonhosted.org/packages/44/b3/12a24488dd0d51498088b755d647eb0546f77919ce6f456fb440cae7c7e2/zeroconf-0.62.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b11ec2e9a039cb153e2b223462ab219085fa52199d2d56e16acb8cf50eae24a1"},
-    {url = "https://files.pythonhosted.org/packages/45/61/61d9c9803edbe750d6024f136244db9dc1b8b4411f4430d608c12e7b45b7/zeroconf-0.62.0-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:e1da206fadbd10a4a8caeaf347a185b9b570744c5e063ac47bc76d27a99712b3"},
-    {url = "https://files.pythonhosted.org/packages/45/b4/ad07260db32651f3e6c4085244b2308237763392ca5dbc88d972fc27e6fb/zeroconf-0.62.0-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:7ea514a329ec63deb470aa859acd3bf4ba4d82d4deba784d8c81ecd5beefb224"},
-    {url = "https://files.pythonhosted.org/packages/4a/bf/773568177e417db780533e14b01f2805c2784522be29510e9fe05dc10312/zeroconf-0.62.0-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:5d76000cb1b8fbe8708d0d801189e32e6f2338f69120333c97e031a925eeb108"},
-    {url = "https://files.pythonhosted.org/packages/4c/e2/02ed4e2589e047913f90ca8b6abee1e0a0f0e8434f6f8cbaa4fb8d8bb922/zeroconf-0.62.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:dfaeae05fba844dc613294e2dc3acebd23e7eee12245b8b0069c959913b94051"},
-    {url = "https://files.pythonhosted.org/packages/52/b6/808b6f78319c7c2cfe18edeea7e5c3a96918fc32f7476cef57572fefa701/zeroconf-0.62.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5ba1bb5a75a0a806376ac3ed000ee7e6806db51a96a52207ffca4ac36cd46d57"},
-    {url = "https://files.pythonhosted.org/packages/54/80/33e0d378ba660e333152a424e0ee1d58d13bbee278c83714999261622e3f/zeroconf-0.62.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6c6f41bc8d9c2f5088dcb4be6e64b0976734825c1e7989a8f92be0d2b40d1167"},
-    {url = "https://files.pythonhosted.org/packages/5d/45/19c5cb4002045c54d62c71264c186a95e27529208868b6eba6bc96ee4346/zeroconf-0.62.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:1a7f65d8b20db5eb28c60ddf199cf388421d2c16086024c2c808ac352e08cf0b"},
-    {url = "https://files.pythonhosted.org/packages/61/2b/2edefd268c7f53fa7e5d2df1f3af7c6a78fe650f4030f5cfd3f86fa57ed9/zeroconf-0.62.0-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:d149513c43b0a7c7cac39bf618f4a436ba9e26334c8d25f1c35d81b69c944c8b"},
-    {url = "https://files.pythonhosted.org/packages/61/9a/86abdc4cf1f1db4c28a64109ffb205af9a3ebb6d100af518c43d875c50e4/zeroconf-0.62.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:70db211ad01e4859beb9f49e71cdcb8828c19ebe5cc475e5b057f1c1cf73bca0"},
-    {url = "https://files.pythonhosted.org/packages/63/e0/8e33581b7db115300d7867462ef84539a9b0ce5dc50e61b00ddee8465bd6/zeroconf-0.62.0-cp38-cp38-macosx_11_0_x86_64.whl", hash = "sha256:d5b02cd16ddd839a05eedc2e775786f0dd30f1dbf4ee3b8844db25382b944752"},
-    {url = "https://files.pythonhosted.org/packages/7a/d2/856d37fac124f1c7461acf88f8c4ff15cd83f3142c5eda7881b23039af1e/zeroconf-0.62.0-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:36da363536a2e16fd29b28045fc04292bae171063260b87abe12fd74db038d7a"},
-    {url = "https://files.pythonhosted.org/packages/83/ed/7585948536dcc87086d5faba0ed005d7608b92c1ade3cc9cbc5503fbff5c/zeroconf-0.62.0-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:9524952b3e865d150daed4156760c7c77c6b108e506985c25d9efcd965e755e9"},
-    {url = "https://files.pythonhosted.org/packages/84/14/23ff01b6d9cc418b823ba4adf566ee3e81b61d9b77c80f39f3885a49c70d/zeroconf-0.62.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:26e2d86e31842a5d8f7df7dc669b6fbda979ec956363206d05572bb04d1d4400"},
-    {url = "https://files.pythonhosted.org/packages/86/8f/fac9aee8152dca745efc18ef65c55907dd52917ee5b5ae00d04beb025d7b/zeroconf-0.62.0.tar.gz", hash = "sha256:c51340a8a7f13d7265dcc582c4a97907c11e4f3d23d5234d3c2c0e44fb446717"},
-    {url = "https://files.pythonhosted.org/packages/99/0a/ba714977b001d4a9948d4b44f5bd4c9cdfd69548a091832516bd0d52fee5/zeroconf-0.62.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:12441c02eee67ef3b5a058d1eeb3c8d18cf5f17c3a50be8c1349ffac03157a2f"},
-    {url = "https://files.pythonhosted.org/packages/a4/28/c437ccdf869de722c2cbe798ffd79c1b16a3941f654fe473bc0773366f5e/zeroconf-0.62.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:347ecd859b45a97fb191b2aa7e3c24281761958e75728ecd5635055dda0b4ecb"},
-    {url = "https://files.pythonhosted.org/packages/d1/0c/40d54fe5bc0ccbd16d4c11e585aab04341a455d2225078044253cfc9121f/zeroconf-0.62.0-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:295cea60fdc2dee509cd8f1e1d31f8c9d09a503cf6a824423fe91102229026b1"},
-    {url = "https://files.pythonhosted.org/packages/d2/c0/7780b2857993604221d64913a630b4384ad71a1ed8ecfb278dfa076500b0/zeroconf-0.62.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:4b0e2fe841a12076ca674ecd16c13e53432504d5f1eae1fcca1f84cd325fc7f2"},
-    {url = "https://files.pythonhosted.org/packages/d3/fe/653717585bf7fdb9d88f39e9bbd85b14cc52d8e72a31aa7e64c7adac5ed2/zeroconf-0.62.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5d151107eafc1480690af42d02483120830f2b4386bb44f60078db0d99e75075"},
-    {url = "https://files.pythonhosted.org/packages/d9/c4/0b1393b42d28bf9b78c420caee41aa5393c9c86c6692d2a6b4e95beb744e/zeroconf-0.62.0-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:64163998a06987780b35744e4e52ef8dbf872801a0faca756f33a270a2e81fc3"},
-    {url = "https://files.pythonhosted.org/packages/df/09/d7c4e55b2c73cbf706dc2c768aac1cccbb34ddc450a32023429e3a68c979/zeroconf-0.62.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:a96e9f8cae73dab2c25bd06ccc668299352773890ca2866c9f58cf8a75ab3d38"},
-    {url = "https://files.pythonhosted.org/packages/e0/29/df795ee3db478ae680ab7c1cf70e6a2acddba0d3461cec53bb5f3198f463/zeroconf-0.62.0-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:eb784bdd12de5642d9570cd8259d0990fb5be1df6b85ecb69fafc1f0614641a5"},
-    {url = "https://files.pythonhosted.org/packages/eb/2a/4ffc605f6834ba714884282a4f5b295fd7f9f42f93958014ecd8dd4c5404/zeroconf-0.62.0-cp37-cp37m-macosx_11_0_x86_64.whl", hash = "sha256:d57764a83465eec9b1e53a91ce2c69c632c8eea63daec712bf4ef3f56c5088d5"},
-    {url = "https://files.pythonhosted.org/packages/ec/f6/bc8ef0b51366210a5a6c65aa80d7ac8e319adbf71f92a99973ae8f062ba8/zeroconf-0.62.0-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:93b43b3a2434325064a24653da18f91a876a70ef7f6aa33340e031b10bc69cbe"},
-    {url = "https://files.pythonhosted.org/packages/ee/24/69eb4865d85d9aff7c96387a8c46c5f45103a21da54d93304a85fa97735b/zeroconf-0.62.0-cp38-cp38-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:68e81a0ef6b5d67d098256420f250dd01aa81d051697eb73d9c9712a063c2d2d"},
-    {url = "https://files.pythonhosted.org/packages/f6/82/894ab528c457dc1ce0f814ca0890b75b3fa79fb5f349fa14e0d94014fb01/zeroconf-0.62.0-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:32380657a1e0ea4e5bdb407cba7bb983e374346008cfac908f977e22fc243407"},
-    {url = "https://files.pythonhosted.org/packages/fb/8a/0bbf7a21dbb32276f4953b0b4a9d1815b43fca6cf9703e6826ff6302cc57/zeroconf-0.62.0-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:80bce57c458d48f179472b5251dd266632978bbb7e5dca47138e9564feaef7bd"},
+"zeroconf 0.63.0" = [
+    {url = "https://files.pythonhosted.org/packages/02/80/9aa80564b42f6d62c3395569b13533e0bef3a5c03ac6df8e5bdc376ff8d4/zeroconf-0.63.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8142e423ce780ef45229ae47f0df8474eb9fab41b6ccea25206330a40c79cbbe"},
+    {url = "https://files.pythonhosted.org/packages/08/77/364326b5600326e115e982fc6bdb53c80e922e35ac0759ffc26cce4cf295/zeroconf-0.63.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:867b0aefd32239e69a7919d95a8bcaf97e3e40fd05c25f5cd5c1e5e50326ca6e"},
+    {url = "https://files.pythonhosted.org/packages/11/f3/c0a9098ee84bfef2eb57b7aca04f244dece53197e0d3cad1e6bea72bb22d/zeroconf-0.63.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:934d468f91885ceb4a530507689c416a1e158a11170f2a90bad3643090c19bac"},
+    {url = "https://files.pythonhosted.org/packages/13/85/4a85da8c81beda97d0a85b81bbcadb66959491fd83dbfa0edcad1bcdb4bc/zeroconf-0.63.0-cp38-cp38-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:ce5ff7ee9e27cd45567d7f9335426c95dd23b3a80f4c47e3edd2db5560861f96"},
+    {url = "https://files.pythonhosted.org/packages/14/fa/d015cd3ad08a137b5e5d6ede2c6da7493dbd47ca0d3f02b2d8efd1313a00/zeroconf-0.63.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:bc4e5fc6e5ac1d9bcf538fdbbbcb4794c8f19039e9cb344a23260507e506cb10"},
+    {url = "https://files.pythonhosted.org/packages/15/0b/e8214d69531f054db380ead35b2ea1c14be1ce19eceb863be6fcc94418b3/zeroconf-0.63.0-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:c360ee0fed2776f4f95008159d59fae1080a91308865297a29941895d8da0de4"},
+    {url = "https://files.pythonhosted.org/packages/19/9a/9cb1ddeedd774e7e1c9350806bbcf8e06af054dc85b7ce9bce5f7877a1c6/zeroconf-0.63.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:fa11e9ee5436c5a4436c72a23bb08e509b38157611eecece0a8e44191129442c"},
+    {url = "https://files.pythonhosted.org/packages/1a/8d/328a856d217f2248a926803309841fdcd1121b8f6c387af5207fe883cf9b/zeroconf-0.63.0-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d9837c1a2952c72b75e906e353801822bde6e0d2521c1572d2c0e39d840d648e"},
+    {url = "https://files.pythonhosted.org/packages/36/53/b51a621fc7b18a8006626e3a2a046f27d98b0f4091e08866c0c082e09947/zeroconf-0.63.0-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:545f433782e2c114b0ab4301d015ee0347036896591238fb0f18433e5eacfc1c"},
+    {url = "https://files.pythonhosted.org/packages/38/ae/b534effd941cc0a2b1cea84b50b2b31f8fe33eb4d439625f3ecc2caaa7e3/zeroconf-0.63.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:a7a6f4afc6c951098f15b9064d5d2b749b64cff8df7f553a5cc38b7b37cce166"},
+    {url = "https://files.pythonhosted.org/packages/41/20/8a12dc796fba28deed4e89417ad7278704b99eace362a98c9253a0b14ad3/zeroconf-0.63.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b864e25bb6cf0d588559caa70177e11bf1bc1c8f78911587cc280f382980c596"},
+    {url = "https://files.pythonhosted.org/packages/46/64/f3f55dc5dba216ce9d20062b6fe5862e49a63b7ecce1c941388618f89224/zeroconf-0.63.0.tar.gz", hash = "sha256:2643b1c9c6ffdfaa1313cf3d12ea0099482fcb3da77929a08be87fc8354d0b3d"},
+    {url = "https://files.pythonhosted.org/packages/50/0f/abab207c6b628ff39cec1bb63ed3469b4aa61eec3b2e6b0bfe45bfe507db/zeroconf-0.63.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:62d634a2e6eb5fd38930ad571d6e44e3095f1482966d7af31470738991c652af"},
+    {url = "https://files.pythonhosted.org/packages/57/54/00e810344ec1be1ad7999438c56a4f7d1f71c2bd5fd860386bce56dd2a11/zeroconf-0.63.0-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:08c91b62f0e21bd55a89718957397d671e439b917404102da2d24acb42e718cb"},
+    {url = "https://files.pythonhosted.org/packages/60/0e/f486a01b052981281c7b376dda078df6b84f817ec3824441cbb3c342d6d7/zeroconf-0.63.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0525f0c1ae03b695c6a1e181e17d35cc563494edb5e12424828f4cb8d7599228"},
+    {url = "https://files.pythonhosted.org/packages/6e/bb/12ddf36fd85db0b15d446ceb740cf1d05d1df205ba84888edf03c519f561/zeroconf-0.63.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:34caa7a1640c84457f517421401214122134a0979046925741d51e881e1012e1"},
+    {url = "https://files.pythonhosted.org/packages/79/54/924592e816205f57d934e02e4175667d9571bd40cb210cd9cef1340b9f5c/zeroconf-0.63.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:e14b99b35d7df8fdc9fa88f3792f523da89eddbc41ad4e3ecc289a42e7145665"},
+    {url = "https://files.pythonhosted.org/packages/8a/f3/526afcb7f35476876fdc55f4256edd974233466d70891e44ff01d610c4c3/zeroconf-0.63.0-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3c293358918fb511aae4ea0602f20845854406cfc6e9606b5b3b5afa7b68a3b4"},
+    {url = "https://files.pythonhosted.org/packages/90/7a/79e216875ef7b59019673fe45b0997eb305ecb5af51371303d0bff8081be/zeroconf-0.63.0-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:18a804537b5cfa96715ed32afac454981dbd152e031d87e2504a6ca24865ff8b"},
+    {url = "https://files.pythonhosted.org/packages/91/43/1aa906bd9cefcd99e64f4dcbb60d693253d5bbd335ae658afd49f44b9635/zeroconf-0.63.0-pp37-pypy37_pp73-macosx_11_0_x86_64.whl", hash = "sha256:2b4c4f256c16129da53553a99a95eaded4e6dd9bd094fcd48478eb7273f7c7c1"},
+    {url = "https://files.pythonhosted.org/packages/9c/e8/03f37a2fb6260db133fc975e159f308345b2d487eea3c1974de28658a3cf/zeroconf-0.63.0-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:be7b119699c2e91d922d4a70fc12514e2b49522e95b17eeddcbca38f3409035b"},
+    {url = "https://files.pythonhosted.org/packages/9e/55/3fb6a4382ce45e61d1ed0ad2027767759e6760fdc7c357be39d29d2326c5/zeroconf-0.63.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e6763fb33a66664b24c0674d0188943e93e7ac6e0e8cf6fe104658f0697bf670"},
+    {url = "https://files.pythonhosted.org/packages/b1/e9/afcae6888a52538082b4659be5308d2804a10e0533934c2cc4c564b786b7/zeroconf-0.63.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6947b13576667122b03b02f580c6f532b134e097efbf1f0660ba84620c6fa4b2"},
+    {url = "https://files.pythonhosted.org/packages/c4/cc/928066b3947f802a412de71df59019d382468c116d3969d332bb4f6e6e4d/zeroconf-0.63.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:f439a5fe58d0c736484017fc49c847e8a00aafe035f199cce35a32b6c76f6e95"},
+    {url = "https://files.pythonhosted.org/packages/c9/9a/6a53221cae1f0233a56137b329945f32b8eda3410b88bcc0f195ed84c8a5/zeroconf-0.63.0-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:23dc430300e78c1515bd2c42fdff1fc813f12f16e6cfe7faccaa89893d193b92"},
+    {url = "https://files.pythonhosted.org/packages/cf/00/6bc23edb28fd1b5d87b993a24326568e721b202545e8c5b309a0ea08136d/zeroconf-0.63.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:764206721e29395b7d5f0427006b168ca1c30cadac6b0414f83c9c62584b1447"},
+    {url = "https://files.pythonhosted.org/packages/d2/26/3cb6925dc295b0a018fb99aeb7e2299a71e48004356e7ff60092e44a73a0/zeroconf-0.63.0-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:a3b2bd53e9c95c9c7f63feb6238fc046866cc86cf511dd64c926836e33ba8f85"},
+    {url = "https://files.pythonhosted.org/packages/e1/39/d4ac426bac2aef9cf3d4e8223905b5aa6f3f18909dc7e4556fdc3d85919e/zeroconf-0.63.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:981c8cce4571733a96d6f6f32b3cde30608f0fb316f073694713b3f18506ba8c"},
+    {url = "https://files.pythonhosted.org/packages/e5/37/7a8b72a5f7a1b0c6a4339c25adbc5a61dbf3c0e3e0cdc4ff897a85f57db9/zeroconf-0.63.0-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:7028ae059f01891a257a83a7c25db266d0c61f963b4f03c905084bf21fcea810"},
+    {url = "https://files.pythonhosted.org/packages/e7/18/f046e990e8055ed324655849a914127b2320699df38cb8b70c121e4f7e05/zeroconf-0.63.0-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:90764ba95fc410cd5da89d6b60c3e5a52a506ac9d841d3f78a95f44ea8ef23f0"},
+    {url = "https://files.pythonhosted.org/packages/eb/11/5ca71b5f173e5fde9180f151bc323c53eba42d2792966edb12cf755a3959/zeroconf-0.63.0-cp38-cp38-macosx_11_0_x86_64.whl", hash = "sha256:664678b9e271a4a6d983366f4241049795f71c0f53025293ed83901d4e19007e"},
+    {url = "https://files.pythonhosted.org/packages/ec/ac/76652d5ffed387d2a43d98a0cb23bdbe3a8c13ca3d7f87aa57ccec1aebe2/zeroconf-0.63.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:d4cd16ccd966d55378737c8ec772795528dc7d58048379c7bc5111a54df38c35"},
+    {url = "https://files.pythonhosted.org/packages/f4/21/f354720c0eee7398b3b81a26913664535a5209af770115ca411b22ec5721/zeroconf-0.63.0-cp37-cp37m-macosx_11_0_x86_64.whl", hash = "sha256:f4d09317893e618cf3dd3b0a56abb2c008f3ae0148ffed8409120a3801ecad8d"},
+    {url = "https://files.pythonhosted.org/packages/f7/10/ceb9a1ff94be25a151dc15724ac95a2b0d9446aff39e9b980908d061402f/zeroconf-0.63.0-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:0ca4d685d441b9acf9c078f0a25d32e9af78a01070afbbf7441084eff90c69bd"},
+    {url = "https://files.pythonhosted.org/packages/f7/7d/6b05abbb1162f02ceb25b94caa3edde44c1aaf10d5d2d2a83563074a89e0/zeroconf-0.63.0-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:a4c68e89762eee873ec949c43c2190f5f6a75380f4648f7dcf0de7463f79e259"},
+    {url = "https://files.pythonhosted.org/packages/ff/a2/4cea466717eea9d33e0a0dedcfe7d01b1f133cdcccebe93f526958bf5b3d/zeroconf-0.63.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2dafe39f657e0d009663332d1a4466666c5047c5f66a6ddacb1a577b1dffac3c"},
 ]
 "zipp 3.15.0" = [
     {url = "https://files.pythonhosted.org/packages/00/27/f0ac6b846684cecce1ee93d32450c45ab607f65c2e0255f0092032d91f07/zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
     {url = "https://files.pythonhosted.org/packages/5b/fa/c9e82bbe1af6266adf08afb563905eb87cab83fde00a0a08963510621047/zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
 ]
```

### Comparing `xklb-1.28.9/readme.py` & `xklb-1.29.1/readme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,53 +1,36 @@
-from xklb import lb, play_actions, scripts
+from xklb import lb, play_actions
+from xklb.scripts.scatter import scatter_usage
 
 print(
     rf"""# xk media library
 
-A wise philosopher once told me: "[the future is autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
+A wise philosopher once told me: "the future is [autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
-Manage large media libraries. An index for your archive.
+Manage and curate large media libraries. An index for your archive.
 Primary usage is local filesystem but also supports some virtual constructs like
 tracking online video playlists (eg. YouTube subscriptions) and scheduling browser tabs.
 
-Required: `ffmpeg`
-
-Recommended: `mpv`, `fish`, `firefox`
-
 ## Install
 
 Linux recommended but [Windows setup instructions](./Windows.md) available.
 
     pip install xklb
 
-## Examples
-
-<details><summary>List all subcommands</summary>
-
-    $ library
-    {lb.usage()}
-
-</details>
-
-### Watch online media on your PC
-
-    wget https://github.com/chapmanjacobd/library/raw/main/examples/mealtime.tw.db
-    library watch mealtime.tw.db
+Should also work on Mac OS.
 
-### Listen to online media on a chromecast group
+### External dependencies
 
-    wget https://github.com/chapmanjacobd/library/raw/main/examples/music.tl.db
-    library listen music.tl.db -ct "House speakers"
+Required: `ffmpeg`
 
-### Hook into HackerNews
+Some features work better with: `mpv`, `firefox`, `fish`
 
-    wget https://github.com/chapmanjacobd/hn_mining/raw/main/hackernews_only_direct.tw.db
-    library watch hackernews_only_direct.tw.db --random --ignore-errors
+## Getting started
 
-## Getting started with local media
+<details><summary>Local media</summary>
 
 ### 1. Extract Metadata
 
 For thirty terabytes of video the initial scan takes about four hours to complete.
 After that, subsequent scans of the path (or any subpaths) are much quicker--only
 new files will be read by `ffprobe`.
 
@@ -59,15 +42,17 @@
 
     library watch tv.db                           # the default post-action is to do nothing
     library watch tv.db --post-action delete      # delete file after playing
     library listen finalists.db -k ask_keep       # ask whether to keep file after playing
 
 To stop playing press Ctrl+C in either the terminal or mpv
 
-## Getting started with online media
+</details>
+
+<details><summary>Online media</summary>
 
 ### 1. Download Metadata
 
 Download playlist and channel metadata. Break free of the YouTube algo~
 
     library tubeadd educational.db https://www.youtube.com/c/BranchEducation/videos
 
@@ -149,28 +134,74 @@
     systemctl --user daemon-reload
     systemctl --user enable --now tabs.service
 
 You can also invoke tabs manually:
 
     library tabs tabs.db -L 1  # open one tab
 
-## Usage
+</details>
+
+<details><summary>List all subcommands</summary>
+
+    $ library
+    {lb.usage()}
+
+</details>
+
+## Examples
+
+### Watch online media on your PC
+
+    wget https://github.com/chapmanjacobd/library/raw/main/examples/mealtime.tw.db
+    library watch mealtime.tw.db
+
+### Listen to online media on a chromecast group
+
+    wget https://github.com/chapmanjacobd/library/raw/main/examples/music.tl.db
+    library listen music.tl.db -ct "House speakers"
+
+### Hook into HackerNews
+
+    wget https://github.com/chapmanjacobd/hn_mining/raw/main/hackernews_only_direct.tw.db
+    library watch hackernews_only_direct.tw.db --random --ignore-errors
+
+## Watch/Listen Usage
 
     $ library watch -h
     usage: {play_actions.usage('watch')}
 
 ## More examples
 
 ### Organize via separate databases.
 
     library fsadd --audio both.db ./audiobooks/ ./podcasts/
     library fsadd --audio audiobooks.db ./audiobooks/
     library fsadd --audio podcasts.db ./podcasts/ ./another/more/secret/podcasts_folder/
 
-### Find large folders to curate or candidates for freeing up space by moving to another mount point
+
+### Find large folders to curate
+
+<details><summary>lb bigdirs</summary>
+
+Also, if you are just looking for folders which are candidates for curation (ie. I need space but don't want to buy a hard drive). The bigdirs subcommand was written for that purpose:
+
+    $ lb bigdirs fs/d.db
+
+You may filter by folder depth (similar to QDirStat or WizTree)
+
+    $ lb bigdirs --depth=3 audio.db
+
+There is also an flag to prioritize folders which have many files which have been deleted (for example you delete songs you don't like--now you can see who wrote those songs and delete all their other songs...)
+
+    $ lb bigdirs --sort-by deleted audio.db
+
+</details>
+
+
+### Find candidates for freeing up space by moving to another mount point
 
 <details><summary>lb mv-list</summary>
 
 The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
 
     $ lb fsadd --filesystem d.db ~/d/
 
@@ -222,37 +253,21 @@
 
         Folder list saved to /tmp/tmpa7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
 
             rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmpa7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
 
 </details>
 
-<details><summary>lb bigdirs</summary>
-
-Also, if you are just looking for folders which are candidates for curation (ie. I need space but don't want to buy a hard drive). The bigdirs subcommand was written for that purpose:
-
-    $ lb bigdirs fs/d.db
-
-You may filter by folder depth (similar to QDirStat or WizTree)
-
-    $ lb bigdirs --depth=3 audio.db
-
-There is also an flag to prioritize folders which have many files which have been deleted (for example you delete songs you don't like--now you can see who wrote those songs and delete all their other songs...)
-
-    $ lb bigdirs --sort-by deleted audio.db
-
-</details>
-
 
 ### Scatter your data across disks with [mergerfs](https://github.com/trapexit/mergerfs)
 
 <details><summary>If you use mergerfs, you'll likely be interested in this</summary>
 
     library scatter -h
-    usage: {scripts.scatter_usage}
+    usage: {scatter_usage}
 
     positional arguments:
     database
     relative_paths        Paths to scatter, relative to the root of your mergerfs mount; any path substring is valid
 
     options:
     -h, --help            show this help message and exit
@@ -274,25 +289,27 @@
     pip install mnamer
     mnamer --movie-directory ~/d/70_Now_Watching/ --episode-directory ~/d/70_Now_Watching/ \
         --no-overwrite -b (library watch -p fd -s 'path : McCloud')
     library fsadd ~/d/70_Now_Watching/
 
 </details>
 
-### Wake up to your own music (via termux)
+### Music alarm clock (via termux crontab)
+
+Wake up to your own music
 
-    30 9 * * * lb listen ./audio.db
+    30 7 * * * lb listen ./audio.db
 
-### Wake up to your own music _only when you are not home_ (computer on local-only IP)
+Wake up to your own music _only when you are *not* home_ (computer on local-only IP)
 
-    30 9 * * * timeout 0.4 nc -z 192.168.1.12 22 || lb listen --random
+    30 7 * * * timeout 0.4 nc -z 192.168.1.12 22 || lb listen --random
 
-### Wake up to your own music on your Chromecast speaker group _only when you are home_
+Wake up to your own music on your Chromecast speaker group _only when you are home_
 
-    30 9 * * * ssh 192.168.1.12 lb listen --random --play-in-order --cast --cast-to "Bedroom pair"
+    30 7 * * * ssh 192.168.1.12 lb listen --cast --cast-to "Bedroom pair"
 
 ### Pipe to [lowcharts](https://github.com/juan-leon/lowcharts)
 
 <details><summary>$ lb watch -p f -col time_created | lowcharts timehist -w 80</summary>
 
     Matches: 445183.
     Each ∎ represents a count of 1896
@@ -325,17 +342,18 @@
 
 ![fps](https://user-images.githubusercontent.com/7908073/184738438-ee566a4b-2da0-4e6d-a4b3-9bfca036aa2a.png)
 
 </details>
 
 ### Pipe to rsync
 
-<details><summary>Copy or move files to your phone via syncthing</summary>
+<details><summary>Move files to your phone via syncthing</summary>
 
-I use rsync to move files instead of copy-on-write duplication because I want deletions to stick.
+I used to use rsync to move files because I want deletions to stick.
+I now use `lb relmv`. But this is still a good rsync example:
 
     function mrmusic
         rsync -a --remove-source-files --files-from=(
             library lt ~/lb/audio.db -s /mnt/d/80_Now_Listening/ -p f \
             --moved /mnt/d/80_Now_Listening/ /mnt/d/ | psub
         ) /mnt/d/80_Now_Listening/ /mnt/d/
```

### Comparing `xklb-1.28.9/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.29.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.29.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/.github/workflows/push.yaml` & `xklb-1.29.1/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/sql/transfer.sql` & `xklb-1.29.1/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/av.py` & `xklb-1.29.1/xklb/av.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 from datetime import datetime, timezone
 from typing import Dict, Optional
 
 import ffmpeg
 
-from xklb import subtitle, utils
+from xklb import consts, subtitle, utils
 from xklb.consts import DBType
 from xklb.utils import combine, log, safe_unpack
 
 
-def get_subtitle_tags(args, f, streams, codec_types) -> dict:
+def get_subtitle_tags(args, path, streams, codec_types) -> dict:
     attachment_count = sum(1 for s in codec_types if s == "attachment")
     internal_subtitles_count = sum(1 for s in codec_types if s == "subtitle")
 
+    subtitles = []
     if args.scan_subtitles:
-        internal_subtitles = subtitle.externalize_internal_subtitles(f, streams)
-        external_subtitles = subtitle.get_external(f)
-        subs_text = subtitle.subs_to_text(f, internal_subtitles + external_subtitles)
+        internal_subtitles = subtitle.externalize_internal_subtitles(path, streams)
+        external_subtitles = subtitle.get_external(path)
+
+        for subtitle_path in internal_subtitles + external_subtitles:
+            try:
+                captions = subtitle.read_sub(subtitle_path)
+            except UnicodeDecodeError:
+                log.warning(f"[{path}] Could not decode subtitle {subtitle_path}")
+            else:
+                subtitles.extend([{"path": path, **d} for d in captions])
     else:
         external_subtitles = []
-        subs_text = []
 
     video_tags = {
         "subtitle_count": internal_subtitles_count + len(external_subtitles),
         "attachment_count": attachment_count,
-        "tags": combine(subs_text),
+        "subtitles": subtitles,
     }
 
     return video_tags
 
 
 def parse_tags(mu: Dict, ti: Dict) -> dict:
     tags = {
@@ -43,16 +50,16 @@
             mu.get("TDOR"),
             mu.get("TORY"),
             mu.get("date"),
             mu.get("TDRC"),
             mu.get("TDRL"),
             ti.get("year"),
         ),
-        "bpm": safe_unpack(mu.get("fBPM"), mu.get("bpm_accuracy")),
-        "key": safe_unpack(mu.get("TIT1"), mu.get("key_accuracy"), mu.get("TKEY")),
+        "bpm": safe_unpack(mu.get("fBPM"), mu.get("bpm"), mu.get("bpm_start")),
+        "key": safe_unpack(mu.get("TIT1"), mu.get("key"), mu.get("TKEY"), mu.get("key_start")),
         "time": combine(mu.get("time_signature")),
         "decade": safe_unpack(mu.get("Songs-DB_Custom1")),
         "categories": safe_unpack(mu.get("Songs-DB_Custom2")),
         "city": safe_unpack(mu.get("Songs-DB_Custom3")),
         "country": combine(
             mu.get("Songs-DB_Custom4"),
             mu.get("MusicBrainz Album Release Country"),
@@ -95,52 +102,62 @@
     except Exception:
         mutagen_tags = {}
 
     stream_tags = parse_tags(mutagen_tags, tiny_tags)
     return stream_tags
 
 
-def munge_av_tags(args, media, f) -> Optional[dict]:
+def munge_av_tags(args, media, path) -> Optional[dict]:
     try:
-        probe = ffmpeg.probe(f, show_chapters=None)
+        probe = ffmpeg.probe(path, show_chapters=None)
     except (KeyboardInterrupt, SystemExit) as sys_exit:
         raise SystemExit(130) from sys_exit
     except Exception as e:
-        log.error(f"[{f}] Failed reading header. Metadata corruption")
+        log.error(f"[{path}] Failed reading header. Metadata corruption")
         log.debug(e)
         if args.delete_unplayable:
-            utils.trash(f)
+            utils.trash(path)
         return None
 
-    if args.check_corrupt or args.delete_corrupt:
-        output = ffmpeg.output(ffmpeg.input(f), "/dev/null", f="null")
-        try:
-            error_log = ffmpeg.run(output, capture_stderr=True)
-        except ffmpeg.Error:
-            log.warning(f"[{f}] Data corruption")
-            if args.delete_corrupt:
-                utils.trash(f)
-
     if "format" not in probe:
-        log.error(f"[{f}] Failed reading format")
+        log.error(f"[{path}] Failed reading format")
         log.warning(probe)
         return None
 
     format_ = probe["format"]
     format_.pop("size", None)
     format_.pop("bit_rate", None)
     format_.pop("format_name", None)
     format_.pop("format_long_name", None)
     format_.pop("nb_programs", None)
     format_.pop("nb_streams", None)
     format_.pop("probe_score", None)
     format_.pop("start_time", None)
     format_.pop("filename", None)
 
-    duration = format_.pop("duration", None)
+    duration = utils.safe_int(format_.pop("duration", None))
+
+    corruption = None
+    if args.check_corrupt and args.check_corrupt > 0.0:
+        if args.check_corrupt >= 100.0:
+            corruption = 0
+            try:
+                utils.decode_full_scan(path)
+            except ffmpeg.Error:
+                corruption = 101
+                log.warning(f"[{path}] Data corruption")
+                if args.delete_corrupt and not consts.PYTEST_RUNNING:
+                    utils.trash(path)
+        else:
+            corruption = utils.decode_quick_scan(path, *utils.cover_scan(duration, args.check_corrupt))
+            if args.delete_corrupt and corruption > args.delete_corrupt:
+                log.warning(f"[{path}] Data corruption ({corruption:.2%}) passed threshold ({args.delete_corrupt:.2%})")
+                if not consts.PYTEST_RUNNING:
+                    utils.trash(path)
+
     tags = format_.pop("tags", None)
     if tags:
         upload_date = tags.get("DATE")
         if upload_date:
             try:
                 upload_date = int(datetime.strptime(upload_date, "%Y%m%d").replace(tzinfo=timezone.utc).timestamp())
             except Exception:
@@ -189,30 +206,40 @@
     height = safe_unpack([s.get("height") for s in streams])
     codec_types = [s.get("codec_type") for s in streams]
     stream_tags = [s.get("tags") for s in streams if s.get("tags") is not None]
     language = combine([t.get("language") for t in stream_tags if t.get("language") not in (None, "und", "unk")])
 
     video_count = sum(1 for s in codec_types if s == "video")
     audio_count = sum(1 for s in codec_types if s == "audio")
-    chapter_count = len(probe["chapters"])
+
+    chapters = getattr(probe, "chapters", [])
+    chapter_count = len(chapters)
+    if chapter_count > 0:
+        chapters = [
+            {"path": path, "time": int(float(d["start_time"])), "text": d["tags"]["title"]}
+            for d in chapters
+            if "tags" in d and "title" in d["tags"] and not utils.is_generic_title(d["tags"]["title"])
+        ]
 
     media = {
         **media,
         "video_count": video_count,
         "audio_count": audio_count,
         "chapter_count": chapter_count,
         "width": width,
         "height": height,
         "fps": fps,
         "duration": 0 if not duration else int(float(duration)),
         "language": language,
+        "corruption": utils.safe_int(corruption),
         **(tags or {}),
+        "chapters": chapters,
     }
 
     if args.profile == DBType.video:
-        video_tags = get_subtitle_tags(args, f, streams, codec_types)
+        video_tags = get_subtitle_tags(args, path, streams, codec_types)
         media = {**media, **video_tags}
 
     if args.profile == DBType.audio:
-        stream_tags = get_audio_tags(f)
+        stream_tags = get_audio_tags(path)
         media = {**media, **stream_tags}
     return media
```

### Comparing `xklb-1.28.9/xklb/books.py` & `xklb-1.29.1/xklb/books.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import re
+import os, re
 from typing import List, Optional
 
 from xklb import utils
 from xklb.utils import combine, log, safe_unpack
 
 REGEX_SENTENCE_ENDS = re.compile(r";|,|\.|\*|\n|\t")
 
 
-def munge_book_tags(media, f) -> Optional[dict]:
+def munge_book_tags(media, path) -> Optional[dict]:
     try:
         import textract
     except ModuleNotFoundError:
         print(
             "textract is required for text database creation: pip install textract; sudo dnf install libxml2-devel libxslt-devel antiword unrtf poppler-utils tesseract sox-plugins-nonfree sox libjpeg-devel swig",
         )
         raise
     try:
-        tags = textract.process(f)
+        tags = textract.process(path, language=os.getenv("TESSERACT_LANGUAGE"))
         tags = REGEX_SENTENCE_ENDS.split(tags.decode())
     except Exception as e:
         log.warning(e)
-        log.error(f"[{f}] Failed reading file")
+        log.error(f"[{path}] Failed reading file")
         tags = []
     return {**media, "tags": combine(tags)}
 
 
 munge_book_tags_fast = utils.with_timeout(70)(munge_book_tags)
 munge_book_tags_slow = utils.with_timeout(350)(munge_book_tags)
```

### Comparing `xklb-1.28.9/xklb/consts.py` & `xklb-1.29.1/xklb/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 DEFAULT_MPV_SOCKET = str(Path(TEMP_DIR) / "mpv_socket")
 DEFAULT_MPV_WATCH_LATER = str(Path("~/.config/mpv/watch_later/").expanduser().resolve())
 SUB_TEMP_DIR = str(Path(TEMP_DIR) / "library_temp_subtitles" / random_string())
 BLOCK_THE_CHANNEL = "__BLOCKLIST_ENTRY_"
 
 LOG_INFO = 1
 LOG_DEBUG = 2
+LOG_DEBUG_SQL = 3
 SIMILAR = 1
 SIMILAR_NO_FILTER = 2
 SIMILAR_NO_FILTER_NO_FTS = 3
+SIMILAR_NO_FILTER_NO_FTS_PARENT = 4
 RELATED = 1
 RELATED_NO_FILTER = 2
 
 SQLITE_PARAM_LIMIT = 32765
 DEFAULT_PLAY_QUEUE = 120
 DEFAULT_MULTIPLE_PLAYBACK = -1
 DEFAULT_SUBTITLE_MIX = 0.35
@@ -88,14 +90,15 @@
     tubeupdate = "tubeupdate"
     tabs = "tabs"
     read = "read"
     view = "view"
     download = "download"
     block = "block"
     stats = "stats"
+    search = "search"
 
 
 class Frequency(enum.Enum):
     Daily = "daily"
     Weekly = "weekly"
     Monthly = "monthly"
     Quarterly = "quarterly"
@@ -178,14 +181,18 @@
     if speech_recognition:
         extensions.extend(SPEECH_RECOGNITION_EXTENSIONS)
 
     return get_files(path, extensions)
 
 
 TUBE_IGNORE_KEYS = (
+    "track_id",
+    "track_number",
+    "repost_count",
+    "fragments",
     "thumbnail",
     "thumbnails",
     "availability",
     "playable_in_embed",
     "is_live",
     "was_live",
     "modified_date",
```

### Comparing `xklb-1.28.9/xklb/data.py` & `xklb-1.29.1/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/db.py` & `xklb-1.29.1/xklb/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,35 +49,38 @@
             except sqlite3.OperationalError as e:
                 if any(ignore_error in str(e) for ignore_error in ignore_errors):
                     return None
                 raise
             return d
 
     if kwargs.get("memory"):
-        db = DB(tracer=tracer if args.verbose >= consts.LOG_DEBUG else None, **kwargs)  # type: ignore
+        db = DB(tracer=tracer if args.verbose >= consts.LOG_DEBUG_SQL else None, **kwargs)  # type: ignore
         return db
 
     if not Path(args.database).exists() and ":memory:" not in args.database:
         log.error(f"Database file '{args.database}' does not exist. Create one with lb fsadd, tubeadd, or tabsadd.")
         raise SystemExit(1)
 
-    db = DB(conn or args.database, tracer=tracer if args.verbose >= consts.LOG_DEBUG else None, **kwargs)  # type: ignore
+    db = DB(conn or args.database, tracer=tracer if args.verbose >= consts.LOG_DEBUG_SQL else None, **kwargs)  # type: ignore
     with db.conn:
         db.conn.execute("PRAGMA main.cache_size = 8000")
 
     db.enable_wal()
     return db
 
 
 config = {
     "media": {
-        "search_columns": ["path", "title", "tags", "mood", "genre", "description", "artist", "album"],
+        "search_columns": ["path", "title", "mood", "genre", "description", "artist", "album"],
         "column_order": ["path", "webpath", "id", "ie_key", "playlist_path"],
         "ignore_columns": ["id"],
     },
+    "captions": {
+        "search_columns": ["text"],
+    },
     "reddit_posts": {
         "search_columns": ["title", "selftext"],
         "column_order": ["playlist_path", "path"],
     },
     "reddit_comments": {
         "search_columns": ["body"],
     },
@@ -171,27 +174,27 @@
 
 
 def fts_quote(query: List[str]) -> List[str]:
     fts_words = [" NOT ", " AND ", " OR ", "*", ":", "NEAR("]
     return [s if any(r in s for r in fts_words) else '"' + s + '"' for s in query]
 
 
-def fts_search(args) -> str:
+def fts_search(args, table="media") -> str:
     args.filter_bindings["query"] = " AND ".join(fts_quote(args.include))
     if args.exclude:
         args.filter_bindings["query"] += " NOT " + " NOT ".join(fts_quote(args.exclude))
-    table = "(" + args.db["media"].search_sql(include_rank=True) + ")"
+    table = "(" + args.db[table].search_sql(include_rank=True) + ")"
     return table
 
 
-def fts_flexible_search(args) -> str:
+def fts_flexible_search(args, table="media") -> str:
     args.filter_bindings["query"] = " OR ".join(fts_quote(args.include))
     if args.exclude:
         args.filter_bindings["query"] += " NOT " + " NOT ".join(fts_quote(args.exclude))
-    table = "(" + args.db["media"].search_sql(include_rank=True) + ")"
+    table = "(" + args.db[table].search_sql(include_rank=True) + ")"
     return table
 
 
 def gen_include_excludes(cols_available):
     searchable_columns = [
         "path",
         "title",
```

### Comparing `xklb-1.28.9/xklb/dl_config.py` & `xklb-1.29.1/xklb/dl_config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 .*Downloading .* manifest
 .*Determining source extension
 .*Downloading jwt token
 .*Skipping embedding .* subtitle because the file is missing
 .*Finished downloading playlist
 .*The last 30x error message was:
 .*NoneType
+.*URL could be a direct video link
 .*unable to download video data
 .*HTTP Error 405
 .*Creating a generic title instead
 .*The channel is not currently live
 .*clips are not currently supported.
 .*Confirm you are on the latest version using
 .*referenced before assignment
@@ -203,15 +204,14 @@
 .*Video unavailable. This video is not available
 .*This article does not contain a video
 .*Resource temporarily unavailable
 .*This video is unavailable
 .*No video could be found in this
 .*Unsupported URL
 .*The requested site is known to use DRM protection.
-.*URL could be a direct video link
 .*No media found
 .*not a valid URL
 .*not a video
 .*The page doesn't contain any tracks
 .*removed by the uploader
 .*Access to this video has been restricted by its creator
 .*blocked due to author's rights infingement
```

### Comparing `xklb-1.28.9/xklb/dl_extract.py` & `xklb-1.29.1/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/fs_extract.py` & `xklb-1.29.1/xklb/fs_extract.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse, math, os, sys
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
+from copy import deepcopy
 from functools import partial
 from multiprocessing import TimeoutError as mp_TimeoutError
 from pathlib import Path
 from shutil import which
 from timeit import default_timer as timer
 from typing import Dict, List, Optional
 
@@ -56,24 +57,28 @@
         const=DBType.image,
         help="Create image database",
     )
     parser.set_defaults(profile=DBType.video)
     parser.add_argument("--scan-all-files", "-a", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
 
-    parser.add_argument("--io-multiplier", default="1")
+    parser.add_argument(
+        "--io-multiplier", type=float, default=1.0, help="Especially useful for text, image, filesystem db types"
+    )
     parser.add_argument("--ocr", "--OCR", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--speech-recognition", "--speech", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--scan-subtitles", "--scan-subtitle", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--extra-media-data", default={})
     parser.add_argument("--extra-playlist-data", default={})
 
     parser.add_argument("--delete-unplayable", action="store_true")
-    parser.add_argument("--check-corrupt", action="store_true")
-    parser.add_argument("--delete-corrupt", action="store_true")
+    parser.add_argument(
+        "--check-corrupt", type=float, default=0.0, help="check that 0 to 100 percent of media decodes correctly"
+    )
+    parser.add_argument("--delete-corrupt", type=float, help="delete media that is more corrupt than this threshold")
     parser.add_argument("--force", "-f", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     if action == SC.fsadd:
         parser.add_argument("paths", nargs="+")
@@ -99,15 +104,14 @@
 
     if args.db:
         args.database = args.db
     Path(args.database).touch()
     args.db = db.connect(args)
     if hasattr(args, "paths"):
         args.paths = utils.conform(args.paths)
-    args.io_multiplier = float(args.io_multiplier)
     log.info(utils.dict_filter_bool(args.__dict__))
 
     if args.profile in (DBType.audio, DBType.video) and not which("ffprobe"):
         log.error("ffmpeg is not installed. Install it with your package manager.")
         raise SystemExit(3)
 
     return args
@@ -118,30 +122,30 @@
         sparseness = 0
     else:
         blocks_allocated = stat.st_blocks * 512
         sparseness = blocks_allocated / stat.st_size
     return sparseness
 
 
-def extract_metadata(mp_args, f) -> Optional[Dict[str, int]]:
-    log.debug(f)
+def extract_metadata(mp_args, path) -> Optional[Dict[str, int]]:
+    log.debug(path)
 
     try:
-        stat = Path(f).stat()
+        stat = Path(path).stat()
     except FileNotFoundError:
         return None
     except OSError:
-        log.error(f"[{f}] IOError: possible filesystem corruption; check dmesg")
+        log.error(f"[{path}] IOError: possible filesystem corruption; check dmesg")
         return None
     except Exception as e:
-        log.error(f"[{f}] %s", e)
+        log.error(f"[{path}] %s", e)
         return None
 
     media = {
-        "path": f,
+        "path": path,
         "play_count": 0,
         "time_played": 0,
         "playhead": 0,
         "size": stat.st_size,
         "time_created": int(stat.st_ctime),
         "time_modified": int(stat.st_mtime) or consts.now(),
         "time_downloaded": consts.APPLICATION_START,
@@ -149,30 +153,30 @@
         "ie_key": "Local",
     }
 
     if hasattr(stat, "st_blocks"):
         media = {**media, "sparseness": calculate_sparseness(stat)}
 
     if mp_args.profile == DBType.filesystem:
-        media = {**media, "is_dir": Path(f).is_dir()}
+        media = {**media, "is_dir": Path(path).is_dir()}
 
     if mp_args.profile in (DBType.audio, DBType.video):
-        media = av.munge_av_tags(mp_args, media, f)
+        media = av.munge_av_tags(mp_args, media, path)
 
     if mp_args.profile == DBType.text:
         try:
             start = timer()
             if any([mp_args.ocr, mp_args.speech_recognition]):
-                media = books.munge_book_tags_slow(media, f)
+                media = books.munge_book_tags_slow(media, path)
             else:
-                media = books.munge_book_tags_fast(media, f)
+                media = books.munge_book_tags_fast(media, path)
         except mp_TimeoutError:
-            log.warning(f"[{f}]: Timed out trying to read file")
+            log.warning(f"[{path}]: Timed out trying to read file")
         else:
-            log.debug(f"[{f}]: {timer()-start}")
+            log.debug(f"[{path}]: {timer()-start}")
 
     return media
 
 
 def clean_up_temp_dirs():
     temp_subs_path = Path(consts.SUB_TEMP_DIR)
     if temp_subs_path.exists():
@@ -183,42 +187,64 @@
 def extract_chunk(args, media) -> None:
     if args.profile == DBType.image:
         media = books.extract_image_metadata_chunk(media)
 
     if args.scan_subtitles:
         clean_up_temp_dirs()
 
+    captions_t0 = []
+    for d in media:
+        chapters = d.pop("chapters", None) or []
+        if len(chapters) > 0:
+            args.db["captions"].insert_all(chapters, alter=True)
+
+        subtitles = d.pop("subtitles", None) or []
+        if len(subtitles) > 0:
+            args.db["captions"].insert_all(subtitles, alter=True)
+
+        tags = d.pop("tags", None) or ""
+        description = d.pop("description", None) or ""
+        if description:
+            tags += "\n" + description
+        if tags:
+            captions_t0.append({"path": d["path"], "time": 0, "text": tags})
+    args.db["captions"].insert_all(captions_t0, alter=True)
+
+    media = utils.list_dict_filter_bool(media)
     args.db["media"].insert_all(utils.list_dict_filter_bool(media), pk="path", alter=True, replace=True)
 
 
 def find_new_files(args, path: Path) -> List[str]:
-    try:
-        if args.scan_all_files:
-            # thanks to these people for making rglob fast https://bugs.python.org/issue26032
-            scanned_files = [str(p) for p in path.rglob("*") if p.is_file()]
-        elif args.profile == DBType.filesystem:
-            scanned_files = [str(p) for p in path.rglob("*")]
-        elif args.profile == DBType.audio:
-            scanned_files = consts.get_audio_files(path)
-        elif args.profile == DBType.video:
-            scanned_files = consts.get_video_files(path)
-        elif args.profile == DBType.text:
-            scanned_files = consts.get_text_files(
-                path,
-                image_recognition=args.ocr,
-                speech_recognition=args.speech_recognition,
-            )
-        elif args.profile == DBType.image:
-            scanned_files = consts.get_image_files(path)
-        else:
-            msg = f"fs_extract for profile {args.profile}"
-            raise NotImplementedError(msg)
-    except FileNotFoundError:
-        print(f"[{path}] Not found")
-        return []
+    if path.is_file():
+        scanned_files = [str(path)]
+    else:
+        try:
+            if args.scan_all_files:
+                # thanks to these people for making rglob fast https://bugs.python.org/issue26032
+                scanned_files = [str(p) for p in path.rglob("*") if p.is_file()]
+            elif args.profile == DBType.filesystem:
+                scanned_files = [str(p) for p in path.rglob("*")]
+            elif args.profile == DBType.audio:
+                scanned_files = consts.get_audio_files(path)
+            elif args.profile == DBType.video:
+                scanned_files = consts.get_video_files(path)
+            elif args.profile == DBType.text:
+                scanned_files = consts.get_text_files(
+                    path,
+                    image_recognition=args.ocr,
+                    speech_recognition=args.speech_recognition,
+                )
+            elif args.profile == DBType.image:
+                scanned_files = consts.get_image_files(path)
+            else:
+                msg = f"fs_extract for profile {args.profile}"
+                raise NotImplementedError(msg)
+        except FileNotFoundError:
+            print(f"[{path}] Not found")
+            return []
 
     columns = args.db["media"].columns_dict
     scanned_set = set(scanned_files)
 
     try:
         deleted_set = {
             d["path"]
@@ -288,16 +314,18 @@
     if not path.exists():
         print(f"[{path}] Path does not exist")
         if args.force:
             player.delete_playlists(args, [str(path)])
         return 0
 
     n_jobs = None
+    if args.check_corrupt > 0:
+        n_jobs = int(min(os.cpu_count() or 2, 2) * args.io_multiplier)
     if args.io_multiplier > 1:
-        n_jobs = int(int(os.cpu_count() or 4) * args.io_multiplier)  # useful for text, image, filesystem db types
+        n_jobs = int(max(os.cpu_count() or 4, 4) * args.io_multiplier)
     if args.verbose >= consts.LOG_DEBUG:
         n_jobs = 1
 
     threadsafe = [DBType.audio, DBType.video, DBType.filesystem]
 
     print(f"[{path}] Building file list...")
     new_files = find_new_files(args, path)
@@ -370,14 +398,25 @@
 
     Create a text database and scan with OCR and speech-recognition:
         library fsadd --text --ocr --speech-recognition ocr.db ./receipts_and_messages/
 
     Create a video database and read internal/external subtitle files into a searchable database:
         library fsadd --scan-subtitles tv.search.db ./tv/ ./movies/
 
+    Decode media to check for corruption (slow):
+        library fsadd --check-corrupt 100 tv.db ./tv/  # scan through 100 percent of each file to evaluate how corrupt it is (very slow)
+        library fsadd --check-corrupt   1 tv.db ./tv/  # scan through 1 percent of each file to evaluate how corrupt it is (takes about one second per file)
+        library fsadd --check-corrupt   5 tv.db ./tv/  # scan through 1 percent of each file to evaluate how corrupt it is (takes about ten seconds per file)
+
+        library fsadd --check-corrupt   5 --delete-corrupt 30 tv.db ./tv/  # scan 5 percent of each file to evaluate how corrupt it is, if 30 percent or more of those checks fail then the file is deleted
+
+        nb: the behavior of delete-corrupt changes between full and partial scan
+        library fsadd --check-corrupt  99 --delete-corrupt  1 tv.db ./tv/  # partial scan 99 percent of each file to evaluate how corrupt it is, if 1 percent or more of those checks fail then the file is deleted
+        library fsadd --check-corrupt 100 --delete-corrupt  1 tv.db ./tv/  # full scan each file to evaluate how corrupt it is, if there is _any_ corruption then the file is deleted
+
     Normally only relevant filetypes are included. You can scan all files with this flag:
         library fsadd --scan-all-files mixed.db ./tv-and-maybe-audio-only-files/
         # I use that with this to keep my folders organized:
         library watch -w 'video_count=0 and audio_count>=1' -pf mixed.db | parallel mv {} ~/d/82_Audiobooks/
 
     Remove path roots with --force
         library fsadd audio.db /mnt/d/Youtube/
```

### Comparing `xklb-1.28.9/xklb/gui.py` & `xklb-1.29.1/xklb/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,33 +108,33 @@
     def move_window(self, window_width=None, window_height=None, x=None, y=None) -> None:
         s_width = window_width or self.root.winfo_screenwidth()
         s_height = window_height or self.root.winfo_screenheight()
 
         # window_width, window_height = 380, 150  # override
         x_coordinate = x or 0
         y_coordinate = y or 0
-        self.root.geometry(f"{window_width}x{window_height}+{x_coordinate}+{y_coordinate}")
+        self.root.geometry(f"{s_width}x{s_height}+{x_coordinate}+{y_coordinate}")
         self.root.update_idletasks()
 
-        log.info(
-            {
-                "winfo_root_x": self.root.winfo_x(),
-                "winfo_root_y": self.root.winfo_y(),
-                "winfo_screen": self.root.winfo_screen(),
-                "wm_maxsize": self.root.wm_maxsize(),
-            },
-        )
+        # log.debug(
+        #     {
+        #         "winfo_root_x": self.root.winfo_x(),
+        #         "winfo_root_y": self.root.winfo_y(),
+        #         "winfo_screen": self.root.winfo_screen(),
+        #         "wm_maxsize": self.root.wm_maxsize(),
+        #     },
+        # )
 
         # TODO: Get the screen which contains the Tk Frame
         # current_screen = self.get_monitor_from_coord(self.winfo_x(), self.winfo_y())
         # current_screen.name
 
-        x_coordinate = x_coordinate + int((s_width / 2) - (window_width / 2))
-        y_coordinate = y_coordinate + int((s_height / 2) - (window_height / 2))
-        self.root.geometry(f"{window_width}x{window_height}+{x_coordinate}+{y_coordinate}")
+        x_coordinate = x_coordinate + int((s_width / 2) - (s_width / 2))
+        y_coordinate = y_coordinate + int((s_height / 2) - (s_height / 2))
+        self.root.geometry(f"{s_width}x{s_height}+{x_coordinate}+{y_coordinate}")
         self.root.wm_attributes("-alpha", 1)
 
     @staticmethod
     def _get_coord_offset_from_monitor(screeninfo_monitor) -> Tuple[int, int]:
         # TODO: assuming screeninfo returns monitors in the same order that Tk is expecting it should
         # be possible to figure out where the monitor sits in the framebuffer then add up the preceding
         # monitors to find the pixel offset within the framebuffer for the window to show up in
```

### Comparing `xklb-1.28.9/xklb/hn_extract.py` & `xklb-1.29.1/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/lb.py` & `xklb-1.29.1/xklb/lb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,35 @@
 import argparse, sys
 
-from xklb import __version__, scripts, utils
+from xklb import __version__, utils
 from xklb.consts import SC
 from xklb.dl_extract import dl_block, dl_download
 from xklb.fs_extract import fs_add, fs_update
 from xklb.hn_extract import hacker_news_add
 from xklb.play_actions import filesystem, listen, read, view, watch
 from xklb.playback import playback_next, playback_now, playback_pause, playback_stop
 from xklb.praw_extract import reddit_add, reddit_update
+from xklb.scripts.bigdirs import bigdirs
+from xklb.scripts.christen import christen
+from xklb.scripts.cluster_sort import cluster_sort
+from xklb.scripts.copy_play_counts import copy_play_counts
+from xklb.scripts.dedupe import dedupe
+from xklb.scripts.merge_dbs import merge_dbs
+from xklb.scripts.merge_online_local import merge_online_local
+from xklb.scripts.mining.extract_links import extract_links
+from xklb.scripts.mining.nouns import nouns
+from xklb.scripts.mining.pushshift import pushshift_extract
+from xklb.scripts.mining.reddit_selftext import reddit_selftext
+from xklb.scripts.move_list import move_list
+from xklb.scripts.optimize_db import optimize_db
+from xklb.scripts.redownload import redownload
+from xklb.scripts.relmv import relmv
+from xklb.scripts.scatter import scatter
+from xklb.scripts.streaming_tab_loader import streaming_tab_loader
+from xklb.search import search
 from xklb.stats import dlstatus, playlists
 from xklb.tabs_actions import tabs
 from xklb.tabs_extract import tabs_add
 from xklb.tube_extract import tube_add, tube_update
 from xklb.utils import log
 
 
@@ -20,14 +38,16 @@
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
+      lb search                Search text and subtitles
+
       lb read                  Read books
       lb view                  View images
 
       lb bigdirs               Discover folders which take much room
       lb dedupe                Deduplicate local db files
       lb relmv                 Move files/folders while preserving relative paths
       lb christen              Cleanse files by giving them a new name
@@ -64,19 +84,22 @@
 
     browser tabs:
       lb tabsadd               Create a tabs database; Add URLs
       lb tabs                  Open your tabs for the day
       lb surf                  Load browser tabs in a streaming way (stdin)
 
     mining:
-      lb extract-links         Extract links from lists of web pages
       lb reddit-selftext       db selftext external links -> db media table
       lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
-      lb nouns                 Unstructured text -> compound nouns (stdin)
       lb hnadd                 Create a hackernews database (this takes a few days)
+
+      lb extract-links         Extract links from lists of web pages
+
+      lb cluster-sort          Lines -> sorted by sentence similarity groups (stdin)
+      lb nouns                 Unstructured text -> compound nouns (stdin)
     """
 
 
 def print_help(parser) -> None:
     print(usage())
     print(parser.epilog)
 
@@ -112,67 +135,70 @@
     subp_fsupdate.set_defaults(func=fs_update)
 
     subp_watch = add_parser(subparsers, SC.watch, ["wt", "tubewatch", "tw", "entries"])
     subp_watch.set_defaults(func=watch)
     subp_listen = add_parser(subparsers, SC.listen, ["lt", "tubelisten", "tl"])
     subp_listen.set_defaults(func=listen)
 
+    subp_search = add_parser(subparsers, "search", ["s"])
+    subp_search.set_defaults(func=search)
+
     subp_read = add_parser(subparsers, SC.read, ["text", "books", "docs"])
     subp_read.set_defaults(func=read)
     subp_view = add_parser(subparsers, SC.view, ["image", "see", "look"])
     subp_view.set_defaults(func=view)
 
     subp_filesystem = add_parser(subparsers, SC.filesystem, ["fs"])
     subp_filesystem.set_defaults(func=filesystem)
 
     subp_bigdirs = add_parser(subparsers, "bigdirs", ["largefolders", "large_folders"])
-    subp_bigdirs.set_defaults(func=scripts.bigdirs)
+    subp_bigdirs.set_defaults(func=bigdirs)
     subp_move_list = add_parser(subparsers, "mv-list", ["movelist", "move-list", "move_list"])
-    subp_move_list.set_defaults(func=scripts.move_list)
+    subp_move_list.set_defaults(func=move_list)
     subp_relmv = add_parser(subparsers, "relmv", ["rel-mv", "mvrel", "mv-rel"])
-    subp_relmv.set_defaults(func=scripts.relmv)
+    subp_relmv.set_defaults(func=relmv)
 
     subp_scatter = add_parser(subparsers, "scatter")
-    subp_scatter.set_defaults(func=scripts.scatter)
+    subp_scatter.set_defaults(func=scatter)
     subp_christen = add_parser(subparsers, "christen")
-    subp_christen.set_defaults(func=scripts.christen)
+    subp_christen.set_defaults(func=christen)
 
     subp_merge_db = add_parser(subparsers, "merge-dbs", ["merge-db", "mergedb", "mergedbs", "merge_db", "merge_dbs"])
-    subp_merge_db.set_defaults(func=scripts.merge_dbs)
+    subp_merge_db.set_defaults(func=merge_dbs)
     subp_merge_db = add_parser(subparsers, "copy-play-counts")
-    subp_merge_db.set_defaults(func=scripts.copy_play_counts)
+    subp_merge_db.set_defaults(func=copy_play_counts)
 
     subp_dedupe = add_parser(subparsers, "dedupe")
-    subp_dedupe.set_defaults(func=scripts.dedupe)
+    subp_dedupe.set_defaults(func=dedupe)
     subp_dedupe_local = add_parser(subparsers, "merge-online-local")
-    subp_dedupe_local.set_defaults(func=scripts.merge_online_local)
+    subp_dedupe_local.set_defaults(func=merge_online_local)
     subp_optimize = add_parser(subparsers, "optimize", ["optimize-db"])
-    subp_optimize.set_defaults(func=scripts.optimize_db)
+    subp_optimize.set_defaults(func=optimize_db)
 
     subp_tubeadd = add_parser(subparsers, "tubeadd", ["dladd", "ta", "da", "xt"])
     subp_tubeadd.set_defaults(func=tube_add)
     subp_tubeupdate = add_parser(subparsers, "tubeupdate", ["dlupdate", "tu"])
     subp_tubeupdate.set_defaults(func=tube_update)
 
     subp_redditadd = add_parser(subparsers, "redditadd", ["ra", "xr"])
     subp_redditadd.set_defaults(func=reddit_add)
     subp_redditupdate = add_parser(subparsers, "redditupdate", ["ru", "xru"])
     subp_redditupdate.set_defaults(func=reddit_update)
     subp_pushshift = add_parser(subparsers, "pushshift", ["ps"])
-    subp_pushshift.set_defaults(func=scripts.pushshift_extract)
+    subp_pushshift.set_defaults(func=pushshift_extract)
 
     subp_hnadd = add_parser(subparsers, "hnadd")
     subp_hnadd.set_defaults(func=hacker_news_add)
 
     subp_download = add_parser(subparsers, "download", ["dl"])
     subp_download.set_defaults(func=dl_download)
     subp_block = add_parser(subparsers, "block")
     subp_block.set_defaults(func=dl_block)
     subp_redownload = add_parser(subparsers, "redownload", ["redl"])
-    subp_redownload.set_defaults(func=scripts.redownload)
+    subp_redownload.set_defaults(func=redownload)
 
     subp_playlist = add_parser(subparsers, "playlists", ["pl", "folders"])
     subp_playlist.set_defaults(func=playlists)
     subp_dlstatus = add_parser(subparsers, "dlstatus", ["ds"])
     subp_dlstatus.set_defaults(func=dlstatus)
     subp_usage = add_parser(subparsers, "usage", ["du"])
     subp_usage.set_defaults(func=utils.mount_stats)
@@ -187,23 +213,25 @@
     subp_playback_pause.set_defaults(func=playback_pause)
 
     subp_tabsadd = add_parser(subparsers, "tabsadd")
     subp_tabsadd.set_defaults(func=tabs_add)
     subp_tabs = add_parser(subparsers, "tabs", ["tb"])
     subp_tabs.set_defaults(func=tabs)
     subp_surf = add_parser(subparsers, "surf", ["browse", "load"])
-    subp_surf.set_defaults(func=scripts.streaming_tab_loader)
+    subp_surf.set_defaults(func=streaming_tab_loader)
 
     subp_nouns = add_parser(subparsers, "nouns")
-    subp_nouns.set_defaults(func=scripts.nouns)
+    subp_nouns.set_defaults(func=nouns)
+    subp_cluster_sort = add_parser(subparsers, "cluster-sort", ["cs", "clustersort", "cluster_sort"])
+    subp_cluster_sort.set_defaults(func=cluster_sort)
 
     subp_reddit_selftext = add_parser(subparsers, "reddit-selftext", ["rst"])
-    subp_reddit_selftext.set_defaults(func=scripts.reddit_selftext)
+    subp_reddit_selftext.set_defaults(func=reddit_selftext)
     subp_nfb_directors = add_parser(subparsers, "extract-links", ["links"])
-    subp_nfb_directors.set_defaults(func=scripts.extract_links)
+    subp_nfb_directors.set_defaults(func=extract_links)
 
     parser.add_argument("--version", "-V", action="store_true")
     return parser
 
 
 def library(args=None) -> None:
     if args:
```

### Comparing `xklb-1.28.9/xklb/play_actions.py` & `xklb-1.29.1/xklb/play_actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import argparse, shlex, shutil, sys, time
 from collections import deque
 from concurrent.futures import ThreadPoolExecutor
-from copy import deepcopy
 from pathlib import Path
 from random import random
-from typing import Dict, Optional, Tuple
+from typing import Dict, Tuple
 
 from xklb import consts, db, player, subtitle, tube_backend, utils
 from xklb.consts import SC
 from xklb.playback import now_playing
-from xklb.player import get_ordinal_media, mark_media_deleted, override_sort
+from xklb.player import mark_media_deleted, override_sort
 from xklb.utils import cmd_interactive, log, random_filename, safe_unpack
 
 
 def usage(action) -> str:
     return f"""library {action} [database] [optional args]
 
     Control playback:
@@ -31,22 +30,29 @@
         library {action} --cast --cast-to "Office pair"
         library {action} -ct "Office pair"  # equivalent
         If you don't know the exact name of your chromecast group run `catt scan`
 
     Play media in order (similarly named episodes):
         library {action} --play-in-order
         There are multiple strictness levels of --play-in-order:
-        library {action} -O   # equivalent
-        library {action} -OO  # above, plus ignores most filters
-        library {action} -OOO # above, plus ignores include/exclude filter during ordinal search
+        library {action} -O    # equivalent
+        library {action} -OO   # above, plus ignores most filters
+        library {action} -OOO  # above, plus ignores fts and (include/exclude) filter during ordinal search
+        library {action} -OOOO # above, plus starts search with parent folder
 
         library {action} --related  # similar to -O but uses fts to find similar content
         library {action} -R         # equivalent
         library {action} -RR        # above, plus ignores most filters
 
+        library {action} --cluster  # cluster-sort to put similar paths closer together
+
+        All of these options can be used together but it will be a bit slow and the results might be mid-tier
+        as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
+        library {action} -RRCOO
+
     Filter media by file siblings of parent directory:
         library {action} --sibling   # only include files which have more than or equal to one sibling
         library {action} --solo      # only include files which are alone by themselves
 
         `--sibling` is just a shortcut for `--lower 2`; `--solo` is `--upper 1`
         library {action} --sibling --solo      # you will always get zero records here
         library {action} --lower 2 --upper 1   # equivalent
@@ -275,73 +281,63 @@
     # switching between videos with and without subs is annoying
     subtitle_count = "=0"
     if random() < getattr(args, "subtitle_mix", consts.DEFAULT_SUBTITLE_MIX):
         # bias slightly toward videos without subtitles
         subtitle_count = ">0"
 
     sorts = [
-        (getattr(args, "random", False), "random", "random"),
-        (args.sort and "rank" in args.sort, args.sort, args.sort),
-        ("video_count" in m_columns and args.action == SC.watch, "video_count > 0 desc", "video_count > 0 "),
-        ("audio_count" in m_columns, "audio_count > 0 desc", "audio_count > 0"),
-        (
-            "time_downloaded" in m_columns and "time_downloaded" not in " ".join(sys.argv),
-            "time_downloaded > 0 desc",
-            "time_downloaded > 0",
-        ),
-        (True, 'm.path like "http%"', 'm.path like "http%" desc'),
-        ("width" in m_columns and hasattr(args, "portrait") and args.portrait, "width < height desc", "width < height"),
-        (
-            "subtitle_count" in m_columns
-            and args.action == SC.watch
-            and not any(
-                [
-                    args.print,
-                    consts.PYTEST_RUNNING,
-                    "subtitle_count" in args.where,
-                    args.limit != consts.DEFAULT_PLAY_QUEUE,
-                ],
-            ),
-            f"subtitle_count {subtitle_count} desc",
-            f"subtitle_count {subtitle_count}",
-        ),
-        (args.sort, args.sort, args.sort),
-        (args.action in (SC.listen, SC.watch) and args.include, "duration desc", "duration"),
-        (args.action in (SC.listen, SC.watch) and args.include, "size desc", "size"),
-        (args.action in (SC.listen, SC.watch) and "play_count" in m_columns, "play_count", "play_count desc"),
-        (
-            args.action in (SC.listen, SC.watch) and "size" in m_columns and "duration" in m_columns,
-            "size desc, duration",
-            "size, duration desc",
-        ),
-        (args.action == SC.filesystem, "sparseness", "sparseness desc"),
-        (args.action == SC.filesystem, "size", "size desc"),
-        (True, "m.path", "m.path desc"),
-        (True, "random", "random"),
+        "random" if getattr(args, "random", False) else None,
+        "rank" if args.sort and "rank" in args.sort else None,
+        "video_count > 0 desc" if "video_count" in m_columns and args.action == SC.watch else None,
+        "audio_count > 0 desc" if "audio_count" in m_columns else None,
+        "time_downloaded > 0 desc"
+        if "time_downloaded" in m_columns and "time_downloaded" not in " ".join(sys.argv)
+        else None,
+        'm.path like "http%"',
+        "width < height desc" if "width" in m_columns and hasattr(args, "portrait") and args.portrait else None,
+        f"subtitle_count {subtitle_count} desc"
+        if "subtitle_count" in m_columns
+        and args.action == SC.watch
+        and not any(
+            [
+                args.print,
+                consts.PYTEST_RUNNING,
+                "subtitle_count" in args.where,
+                args.limit != consts.DEFAULT_PLAY_QUEUE,
+            ],
+        )
+        else None,
+        args.sort,
+        "duration desc" if args.action in (SC.listen, SC.watch) and args.include else None,
+        "size desc" if args.action in (SC.listen, SC.watch) and args.include else None,
+        "play_count" if args.action in (SC.listen, SC.watch) and "play_count" in m_columns else None,
+        "size desc, duration"
+        if args.action in (SC.listen, SC.watch) and "size" in m_columns and "duration" in m_columns
+        else None,
+        "sparseness" if args.action == SC.filesystem else None,
+        "size" if args.action == SC.filesystem else None,
+        "m.path",
+        "random",
     ]
 
-    sort = [
-        c[2] if args.print and "f" not in args.print and "limit" in getattr(args, "defaults", []) else c[1]
-        for c in sorts
-        if c[0]
-    ]
-    sort = list(filter(bool, sort))
+    sort = list(filter(bool, sorts))
     sort = [override_sort(s) for s in sort]
     sort = "\n        , ".join(sort)
     args.sort = sort.replace(",,", ",")
 
 
 def parse_args(action, default_chromecast=None) -> argparse.Namespace:
     DEFAULT_PLAYER_ARGS_SUB = ["--speed=1"]
     DEFAULT_PLAYER_ARGS_NO_SUB = ["--speed=1.46"]
 
     parser = argparse.ArgumentParser(prog="library " + action, usage=usage(action))
 
     parser.add_argument("--play-in-order", "-O", action="count", default=0, help=argparse.SUPPRESS)
     parser.add_argument("--related", "-R", action="count", default=0, help=argparse.SUPPRESS)
+    parser.add_argument("--cluster", "-C", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
     parser.add_argument("--random", "-r", action="store_true", help=argparse.SUPPRESS)
 
     parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--include", "-s", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--no-fts", action="store_true")
@@ -379,16 +375,14 @@
     parser.add_argument("--screen-name", help=argparse.SUPPRESS)
     parser.add_argument("--crop", "--zoom", "--stretch", "--fit", "--fill", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--hstack", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--vstack", action="store_true", help=argparse.SUPPRESS)
 
     parser.add_argument("--portrait", "-portrait", action="store_true", help=argparse.SUPPRESS)
 
-    parser.add_argument("--prefix", default="", help=argparse.SUPPRESS)
-
     parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
     parser.add_argument("--size", "-S", action="append", help=argparse.SUPPRESS)
     parser.add_argument("--duration-from-size", action="append", help=argparse.SUPPRESS)
 
     parser.add_argument("--print", "-p", default=False, const="p", nargs="?", help=argparse.SUPPRESS)
     parser.add_argument("--moved", nargs=2, help=argparse.SUPPRESS)
 
@@ -432,16 +426,32 @@
     parser.add_argument("--solo", action="store_true")
 
     parser.add_argument("--sort-by", action="store_true")
     parser.add_argument("--depth", "-D", default=0, type=int, help="Depth of folders")
     parser.add_argument("--lower", type=int, help="Number of files per folder lower limit")
     parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
 
-    parser.add_argument("--timeout", "-T", help=argparse.SUPPRESS)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
+    parser.add_argument("--prefix", default="", help=argparse.SUPPRESS)
+    parser.add_argument(
+        "--folder",
+        action="store_true",
+        help="Experimental escape hatch to open folder which breaks a lot of features like post-actions",
+    )
+    parser.add_argument(
+        "--folder-glob",
+        "--folderglob",
+        type=int,
+        default=False,
+        const=10,
+        nargs="?",
+        help="Experimental escape hatch to open a folder glob limited to x number of files; breaks a lot of features like post-actions",
+    )
+
+    parser.add_argument("--timeout", "-T", help="Quit after x minutes")
+    parser.add_argument("--db", "-db", help="Override the positional argument database location")
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true")
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
     parser.add_argument("database")
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
     args.action = action
@@ -562,15 +572,15 @@
         args.filter_sql.append(
             f"and time_deleted < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_before)}')) as int)",
         )
 
     args.table = "media"
     if args.db["media"].detect_fts() and not args.no_fts:
         if args.include:
-            args.table = db.fts_search(args)
+            args.table = db.fts_flexible_search(args)
             m_columns = {**m_columns, "rank": int}
         elif args.exclude:
             db.construct_search_bindings(args, m_columns)
     else:
         db.construct_search_bindings(args, m_columns)
 
     if args.table == "media" and not any(
@@ -604,20 +614,21 @@
         args.select += "cast(length(tags) / 4.2 / 220 * 60 as INT) + 10 duration"
     args.select_sql = "\n        , ".join(args.select)
     args.limit_sql = "LIMIT " + str(args.limit) if args.limit else ""
     args.offset_sql = f"OFFSET {args.skip}" if args.skip and args.limit else ""
     query = f"""WITH m as (
     SELECT rowid, * FROM {args.table}
     WHERE 1=1
-        {" ".join(args.filter_sql)}
         {player.filter_args_sql(args, m_columns)}
     )
     SELECT
         {args.select_sql}
     FROM m
+    WHERE 1=1
+        {" ".join(args.filter_sql)}
     ORDER BY 1=1
         , {args.sort}
     {args.limit_sql} {args.offset_sql}
     """
 
     args.filter_sql = [
         s for s in args.filter_sql if "rowid" not in s
@@ -638,23 +649,14 @@
         if catt_log.stderr is None or catt_log.stderr == "":
             if not args.cast_with_local:
                 raise RuntimeError("catt does not exit nonzero? but something might have gone wrong")
         elif "Heartbeat timeout, resetting connection" in catt_log.stderr:
             raise RuntimeError("Media is possibly partially unwatched")
 
 
-def is_play_in_order_lvl2(args, media_file) -> bool:
-    return any(
-        [
-            args.play_in_order >= consts.SIMILAR,
-            args.action == SC.listen and "audiobook" in media_file.lower(),
-        ],
-    )
-
-
 def transcode(args, path) -> str:
     log.debug(path)
     sub_index = subtitle.get_sub_index(args, path)
 
     transcode_dest = str(Path(path).with_suffix(".mkv"))
     temp_video = random_filename(transcode_dest)
 
@@ -709,15 +711,15 @@
 
 
 def prep_media(args, m: Dict, ignore_paths):
     t = utils.Timer()
     args.db = db.connect(args)
     log.debug("db.connect: %s", t.elapsed())
 
-    if is_play_in_order_lvl2(args, m["path"]):
+    if (args.play_in_order >= consts.SIMILAR) or (args.action == SC.listen and "audiobook" in m["path"].lower()):
         m = player.get_ordinal_media(args, m, ignore_paths)
         log.debug("player.get_ordinal_media: %s", t.elapsed())
 
     m["original_path"] = m["path"]
     if not m["path"].startswith("http"):
         media_path = Path(args.prefix + m["path"]).resolve() if args.prefix else Path(m["path"])
         m["path"] = str(media_path)
@@ -795,14 +797,15 @@
         [
             args.partial,
             args.lower,
             args.upper,
             args.safe,
             args.play_in_order >= consts.SIMILAR,
             args.related >= consts.RELATED,
+            args.cluster,
         ]
     ):
         player.printer(args, query, bindings)
         return
 
     media = list(args.db.query(query, bindings))
     log.debug("query: %s", t.elapsed())
@@ -819,48 +822,57 @@
         utils.no_media_found()
 
     if all(
         [
             Path(args.watch_later_directory).exists(),
             args.play_in_order == 0,
             args.related == 0,
+            not args.cluster,
             "sort" in args.defaults,
             not args.partial,
             not args.random,
         ],
     ):
         media = utils.mpv_enrich(args, media)
         log.debug("utils.mpv_enrich: %s", t.elapsed())
 
     if args.safe:
         media = [d for d in media if tube_backend.is_supported(d["path"]) or Path(d["path"]).exists()]
         log.debug("tube_backend.is_supported: %s", t.elapsed())
 
+    if args.related >= consts.RELATED:
+        media = player.get_related_media(args, media[0])
+        log.debug("player.get_related_media: %s", t.elapsed())
+
+    if args.cluster:
+        media_keyed = {d["path"]: d for d in media}
+        groups = utils.cluster_paths([d["path"] for d in media])
+        groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_prefix"])))
+        sorted_paths = utils.flatten(d["grouped_paths"] for d in groups)
+        media = [media_keyed[p] for p in sorted_paths]
+
     if args.print:
-        if args.related >= consts.RELATED:
-            media = player.get_related_media(args, media[0])
         if args.play_in_order >= consts.SIMILAR:
             media = [player.get_ordinal_media(args, d) for d in media]
         player.media_printer(args, media)
     elif args.multiple_playback:
         args.gui = True
         player.multiple_player(args, media)
     else:
-        if args.related >= consts.RELATED:
-            media = player.get_related_media(args, media[0])
-            log.debug("player.get_related_media: %s", t.elapsed())
         try:
             mp_args = argparse.Namespace(**{k: v for k, v in args.__dict__.items() if k not in {"db"}})
             media.reverse()  # because media.pop()
             ignore_paths = []
             futures = deque()
             with ThreadPoolExecutor(max_workers=1) as executor:
                 while media or futures:
                     while media and len(futures) < 3:
                         m = media.pop()
+                        if m["path"] in ignore_paths:
+                            continue
                         future = executor.submit(prep_media, mp_args, m, ignore_paths)
                         ignore_paths.append(m["path"])
                         futures.append(future)
 
                     if futures:
                         future = futures.popleft()
                         m = future.result()
```

### Comparing `xklb-1.28.9/xklb/playback.py` & `xklb-1.29.1/xklb/playback.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,21 +31,14 @@
         "catt": Path(consts.CAST_NOW_PLAYING).read_text() if Path(consts.CAST_NOW_PLAYING).exists() else None,
         "mpv": args.mpv.command("get_property", "path") if Path(args.mpv_socket).exists() else None,
     }
     log.info(media)
     return media
 
 
-def indent_prefix_first(text, prefix, indent="\t"):
-    lines = text.splitlines()
-    first_line = textwrap.indent(lines[0], prefix + indent) + "\n"
-    rest_lines = textwrap.indent("\n".join(lines[1:]), indent)
-    return first_line + rest_lines
-
-
 def now_playing(path) -> str:
     if path.startswith("http"):
         text = path
     else:
         text = (
             path
             + "\n"
@@ -64,14 +57,21 @@
             text = path
             text.encode()
             return text
         except Exception:
             return "Could not encode file path as UTF-8"
 
 
+def indent_prefix_first(text, prefix, indent="\t"):
+    lines = text.splitlines()
+    first_line = textwrap.indent(lines[0], prefix + indent) + "\n"
+    rest_lines = textwrap.indent("\n".join(lines[1:]), indent)
+    return first_line + rest_lines
+
+
 def source_now_playing(playing, source) -> str:
     path = playing[source]
     text = indent_prefix_first(now_playing(path), prefix=source)
     return text
 
 
 def playback_now() -> None:
```

### Comparing `xklb-1.28.9/xklb/player.py` & `xklb-1.29.1/xklb/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import csv, operator, os, platform, re, shutil, socket, subprocess, sys
+import csv, os, platform, re, shutil, socket, statistics, subprocess, sys
 from copy import deepcopy
 from io import StringIO
 from numbers import Number
 from pathlib import Path
 from platform import system
 from random import randrange
 from shlex import join, quote, split
@@ -10,15 +10,15 @@
 from time import sleep
 from typing import Dict, List, Optional, Tuple, Union
 
 from tabulate import tabulate
 
 from xklb import consts, db, utils
 from xklb.consts import SC
-from xklb.scripts import process_bigdirs
+from xklb.scripts.bigdirs import process_bigdirs
 from xklb.utils import cmd, cmd_interactive, human_time, log
 
 try:
     import tkinter  # noqa
 
     from xklb import gui
 except ModuleNotFoundError:
@@ -105,24 +105,24 @@
             player.extend([f"--input-ipc-server={args.mpv_socket}", "--no-video", "--keep-open=no", "--really-quiet"])
         elif args.action in (SC.watch):
             player.extend(["--force-window=yes", "--really-quiet"])
 
         if m["path"] and m["path"].startswith("http"):
             player.extend(["--script-opts=ytdl_hook-try_ytdl_first=yes"])
 
-        if not args.multiple_playback:
+        if getattr(args, "multiple_playback", 1) < 2:
             player.extend(["--fs"])
 
         if args.loop:
             player.extend(["--loop-file=inf"])
 
-        if args.crop:
+        if getattr(args, "crop", None):
             player.extend(["--panscan=1.0"])
 
-        if args.action in (SC.watch, SC.listen) and m:
+        if args.action in (SC.watch, SC.listen, SC.search) and m:
             start, end = calculate_duration(args, m)
             if end != 0:
                 if start != 0:
                     player.extend([f"--start={start}", "--no-save-position-on-quit"])
                 if end != m["duration"]:
                     player.extend([f"--end={end}"])
 
@@ -368,48 +368,54 @@
         sort_expression.replace("month_created", year_month_sql("time_created"))
         .replace("month_modified", year_month_sql("time_modified"))
         .replace("random", "random()")
         .replace("priority", "ntile(1000) over (order by size) desc, duration")
     )
 
 
+def filter_args_sql(args, m_columns):
+    return f"""
+        {'and path like "http%"' if getattr(args, 'safe', False) else ''}
+        {f'and path not like "{args.keep_dir}%"' if getattr(args, 'keep_dir', False) and Path(args.keep_dir).exists() else ''}
+        {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns and 'time_deleted' not in ' '.join(sys.argv) else ''}
+        {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
+        {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
+        {'AND COALESCE(time_downloaded,0) = 0' if args.online_media_only else ''}
+        {'AND COALESCE(time_downloaded,1)!= 0 AND path not like "http%"' if args.local_media_only else ''}
+    """
+
+
 def last_chars(candidate) -> str:
     remove_groups = re.split(r"([\W]+|\s+|Ep\d+|x\d+|\.\d+)", candidate)
     log.debug(remove_groups)
 
     remove_chars = ""
     number_of_groups = 1
     while len(remove_chars) < 1:
         remove_chars += remove_groups[-number_of_groups]
         number_of_groups += 1
 
     return remove_chars
 
 
-def filter_args_sql(args, m_columns):
-    return f"""
-        {'and path like "http%"' if args.safe else ''}
-        {f'and path not like "{args.keep_dir}%"' if Path(args.keep_dir).exists() else ''}
-        {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns and 'time_deleted' not in ' '.join(sys.argv) else ''}
-        {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
-        {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
-        {'AND COALESCE(time_downloaded,0) = 0' if args.online_media_only else ''}
-        {'AND COALESCE(time_downloaded,1)!= 0 AND path not like "http%"' if args.local_media_only else ''}
-    """
-
-
 def get_ordinal_media(args, m: Dict, ignore_paths=None) -> Dict:
     # TODO: maybe try https://dba.stackexchange.com/questions/43415/algorithm-for-finding-the-longest-prefix
     if ignore_paths is None:
         ignore_paths = []
 
     m_columns = args.db["media"].columns_dict
 
+    cols = args.cols or ["path", "title", "duration", "size", "subtitle_count", "is_dir"]
+    args.select_sql = "\n        , ".join([c for c in cols if c in m_columns or c in ["*"]])
+
     total_media = args.db.execute("select count(*) val from media").fetchone()[0]
     candidate = deepcopy(m["path"])
+    if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS_PARENT:
+        candidate = str(Path(candidate).parent)
+
     similar_videos = []
     while len(similar_videos) <= 1:
         if candidate == "":
             return m
 
         remove_chars = last_chars(candidate)
 
@@ -443,20 +449,21 @@
         similar_videos = list(args.db.query(query, bindings))
         log.debug(similar_videos)
 
         TOO_MANY_SIMILAR = 99
         if len(similar_videos) > TOO_MANY_SIMILAR or len(similar_videos) == total_media:
             return m
 
-        commonprefix = os.path.commonprefix([d["path"] for d in similar_videos])
-        log.debug(commonprefix)
-        PREFIX_LENGTH_THRESHOLD = 3
-        if len(Path(commonprefix).name) < PREFIX_LENGTH_THRESHOLD:
-            log.debug("Using commonprefix")
-            return m
+        if len(similar_videos) > 0:
+            commonprefix = os.path.commonprefix([d["path"] for d in similar_videos])
+            log.debug(commonprefix)
+            PREFIX_LENGTH_THRESHOLD = 3
+            if len(Path(commonprefix).name) < PREFIX_LENGTH_THRESHOLD:
+                log.debug("Using commonprefix")
+                return m
 
     return similar_videos[0]
 
 
 def get_related_media(args, m: Dict) -> List[Dict]:
     m_columns = args.db["media"].columns_dict
     m_columns.update(rank=int)
@@ -464,17 +471,14 @@
     m = args.db["media"].get(m["path"])
     words = set(
         utils.conform(utils.extract_words(m.get(k)) for k in m.keys() if k in db.config["media"]["search_columns"])
     )
     args.include = sorted(words, key=len, reverse=True)[:100]
     args.table = db.fts_flexible_search(args)
 
-    cols = args.cols or ["path", "title", "duration", "size", "subtitle_count", "is_dir", "rank"]
-    args.select = [c for c in cols if c in m_columns or c in ["*"]]
-    args.select_sql = "\n        , ".join(args.select)
     query = f"""
         SELECT
             {args.select_sql}, rank
         FROM {args.table} m
         WHERE 1=1
             and path != :path
             {filter_args_sql(args, m_columns)}
@@ -775,45 +779,83 @@
             sleep(0.2)  # I don't know if this is necessary but may as well~~
     finally:
         for m in players:
             m["process"].kill()
 
 
 def local_player(args, m) -> subprocess.CompletedProcess:
+    if args.folder:
+        paths = [str(Path(m["path"]).parent)]
+    elif args.folder_glob:
+        paths = utils.fast_glob(Path(m["path"]).parent, args.folder_glob)
+    else:
+        paths = [m["path"]]
+
     if system() == "Windows" or args.action in (SC.watch):
-        r = cmd(*args.player, m["path"], strict=False)
+        r = cmd(*args.player, *paths, strict=False)
     else:  # args.action in (SC.listen)
-        r = cmd_interactive(*args.player, m["path"])
+        r = cmd_interactive(*args.player, *paths)
 
     if args.player_need_sleep:
-        if hasattr(m, "duration"):
-            delay = m["duration"]
-        else:
-            delay = 10  # TODO: idk
-        sleep(delay)
+        try:
+            utils.confirm("Continue?")
+        except Exception:
+            if hasattr(m, "duration"):
+                delay = m["duration"]
+            else:
+                delay = 10  # TODO: idk
+            sleep(delay)
 
     return r
 
 
+def historical_usage(args):
+    query = """
+    SELECT
+        strftime('%Y-%m-%d', datetime(time_played, 'unixepoch')) AS day
+        , SUM(duration) AS duration_sum
+        , AVG(duration) AS duration_avg
+        , SUM(size) AS size_sum
+        , AVG(size) AS size_avg
+    FROM media where time_played>0
+    GROUP BY day
+    """
+    return list(args.db.query(query))
+
+
+def cadence_adjusted_duration(args, duration):
+    try:
+        historical_daily = statistics.mean((d["duration_sum"] or 0) for d in historical_usage(args))
+    except statistics.StatisticsError:
+        return duration
+
+    return duration / historical_daily * 86400
+
+
 def media_printer(args, media) -> None:
     if "b" in args.print:
         media = process_bigdirs(args, media)
 
     if args.verbose >= consts.LOG_DEBUG and args.cols and "*" in args.cols:
         breakpoint()
 
     if not media:
         utils.no_media_found()
 
+    if "f" not in args.print and "limit" in getattr(args, "defaults", []):
+        media.reverse()
+
+    duration = sum(m.get("duration") or 0 for m in media)
     if "a" in args.print:
         D = {"path": "Aggregate", "count": len(media)}
 
         if "duration" in media[0]:
-            D["duration"] = sum((d["duration"] or 0) for d in media)
-            D["avg_duration"] = sum((d["duration"] or 0) for d in media) / len(media)
+            D["duration"] = duration
+            D["avg_duration"] = duration / len(media)
+            D["cadence_adj_duration"] = cadence_adjusted_duration(args, duration)
 
         if "sparseness" in media[0]:
             D["sparseness"] = None
 
         if "size" in media[0]:
             D["size"] = sum((d["size"] or 0) for d in media)
             D["avg_size"] = sum((d["size"] or 0) for d in media) / len(media)
@@ -823,27 +865,27 @@
                 if isinstance(media[0][c], Number):
                     D[f"sum_{c}"] = sum((d[c] or 0) for d in media)
                     D[f"avg_{c}"] = sum((d[c] or 0) for d in media) / len(media)
         media = [D]
 
     else:
         if "d" in args.print:
-            marked = mark_media_deleted(args, list(map(operator.itemgetter("path"), media)))
+            marked = mark_media_deleted(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as deleted")
         if "w" in args.print:
-            marked = mark_media_watched(args, list(map(operator.itemgetter("path"), media)))
+            marked = mark_media_watched(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as watched")
 
     if "f" in args.print:
         if args.limit == 1:
-            f = media[0]["path"]
-            if not Path(f).exists():
-                mark_media_deleted(args, f)
+            path = media[0]["path"]
+            if not Path(path).exists():
+                mark_media_deleted(args, path)
                 raise FileNotFoundError
-            utils.pipe_print(quote(f))
+            utils.pipe_print(quote(path))
             return
         else:
             if not args.cols:
                 args.cols = ["path"]
 
             selected_cols = [{k: d.get(k, None) for k in args.cols} for d in media]
             virtual_csv = StringIO()
@@ -854,36 +896,36 @@
             virtual_csv.seek(0)
             for line in virtual_csv.readlines():
                 if args.moved:
                     utils.pipe_print(line.strip().replace(args.moved[0], "", 1))
                 else:
                     utils.pipe_print(line.strip())
             if args.moved:
-                moved_media(args, list(map(operator.itemgetter("path"), media)), *args.moved)
+                moved_media(args, [d["path"] for d in media], *args.moved)
                 return
             return
     else:
         tbl = deepcopy(media)
         utils.col_resize(tbl, "path", 22)
         utils.col_resize(tbl, "title", 11)
 
         utils.col_naturalsize(tbl, "size")
         utils.col_naturalsize(tbl, "avg_size")
         utils.col_duration(tbl, "duration")
         utils.col_duration(tbl, "avg_duration")
+        utils.col_duration(tbl, "cadence_adj_duration")
 
         for t in consts.TIME_COLUMNS:
             utils.col_naturaldate(tbl, t)
 
         print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
         if len(media) > 1:
             print(f"{len(media)} media" + (f" (limited to {args.limit})" if args.limit else ""))
 
-        duration = sum(m.get("duration") or 0 for m in media)
         if duration > 0:
             duration = human_time(duration)
             if "a" not in args.print:
                 print("Total duration:", duration)
                 return
             return
         return
```

### Comparing `xklb-1.28.9/xklb/praw_extract.py` & `xklb-1.29.1/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/stats.py` & `xklb-1.29.1/xklb/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, json, operator
+import argparse, json
 from copy import deepcopy
 from typing import Tuple
 
 from tabulate import tabulate
 
 from xklb import consts, db, dl_extract, play_actions, tube_backend, utils
 from xklb.player import delete_playlists
@@ -57,15 +57,15 @@
     args.filter_bindings = {}
 
     args.filter_sql.extend([" and " + w for w in args.where])
 
     args.table = "playlists"
     if args.db["playlists"].detect_fts():
         if args.include:
-            args.table = db.fts_search(args)
+            args.table = db.fts_flexible_search(args)
         elif args.exclude:
             db.construct_search_bindings(args, pl_columns)
     else:
         db.construct_search_bindings(args, pl_columns)
 
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     query = f"""SELECT
@@ -94,15 +94,15 @@
     tbl = deepcopy(media)
     utils.col_naturaldate(tbl, "avg_time_since_download")
     utils.col_naturalsize(tbl, "size")
     utils.col_duration(tbl, "duration")
     utils.col_duration(tbl, "avg_playlist_duration")
 
     if args.fields:
-        pipe_print("\n".join(list(map(operator.itemgetter("path"), media))))
+        pipe_print("\n".join([d["path"] for d in media]))
         return
     elif args.json or consts.TERMINAL_SIZE.columns < 80:
         print(json.dumps(tbl, indent=3))
     else:
         tbl = utils.col_resize(tbl, "path", 30)
         tbl = utils.col_resize(tbl, "title", 20)
         tbl = utils.col_resize(tbl, "uploader_url")
```

### Comparing `xklb-1.28.9/xklb/subtitle.py` & `xklb-1.29.1/xklb/subtitle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-import tempfile
+import re, tempfile
 from pathlib import Path
 from typing import List, Optional
 
 import ffmpeg
 
 from xklb import db, utils
 from xklb.consts import SUB_TEMP_DIR
 from xklb.utils import flatten, log, remove_consecutive_whitespace, remove_text_inside_brackets
 
 SUBTITLE_FORMATS = "vtt|srt|ssa|ass|jss|aqt|mpl2|mpsub|pjs|rt|sami|smi|stl|xml|txt|psb|ssf|usf"
 IMAGE_SUBTITLE_CODECS = ["dvbsub", "dvdsub", "pgssub", "xsub", "dvb_subtitle", "dvd_subtitle", "hdmv_pgs_subtitle"]
+SUBSTATION_OVERRIDE_TAG = re.compile(r"{[^}]*}")
 
 
-def extract(video_file, stream_index) -> Optional[str]:
+def extract_from_video(path, stream_index) -> Optional[str]:
     Path(SUB_TEMP_DIR).mkdir(parents=True, exist_ok=True)
     temp_srt = tempfile.mktemp(".srt", dir=SUB_TEMP_DIR)
 
     stream_id = "0:" + str(stream_index)
 
     try:
-        ffmpeg.input(video_file).output(temp_srt, map=stream_id).global_args("-nostdin").run(quiet=True)
+        ffmpeg.input(path).output(temp_srt, map=stream_id).global_args("-nostdin").run(quiet=True)
     except ffmpeg.Error as e:
         log.info(
             f"Could not extract subtitle {stream_id} from video file. Likely incorrect subtitle character encoding set. %s",
-            video_file,
+            path,
         )
         log.debug(e.stderr.decode())
         return None
 
     return temp_srt
 
 
@@ -40,55 +41,72 @@
         log.info("Could not convert subtitle")
         log.info(e.stderr.decode())
         raise UnicodeDecodeError("utf-8", b"Dr. John A. Zoidberg", 1, 2, "Bleh!") from e
 
     return temp_srt
 
 
-def read_sub_unsafe(path) -> List[str]:
+def ssa_to_markdown(text):
+    tag_replacements = {
+        r"{\\i1}": "*",  # Italic
+        r"{\\b1}": "**",  # Bold
+        r"{\\u1}": "<u>",  # Underline
+        r"{\\s1}": "~~",  # Strikeout
+    }
+    for tag, replacement in tag_replacements.items():
+        text = re.sub(re.escape(tag), replacement, text)
+
+    text = SUBSTATION_OVERRIDE_TAG.sub("", text)
+    text = text.replace(r"\h", " ").replace(r"\n", "\n").replace(r"\N", "\n").replace("\n", " ")
+    return text
+
+
+def read_sub_unsafe(path):
     import pysubs2
 
-    return [
-        remove_text_inside_brackets(caption.text.replace(r"\N", " ").replace(r"\n", " ").replace("\n", " "))
-        for caption in pysubs2.load(path, format_="srt")
-    ]
+    subs = pysubs2.load(path, format_="srt")
+    subs.remove_miscellaneous_events()
+    subs.sort()
+
+    combined_captions = {}
+    for caption in subs:
+        text = remove_consecutive_whitespace(ssa_to_markdown(caption.text).strip())
+        if remove_text_inside_brackets(text):
+            start_time = caption.start // 1000
+            if start_time in combined_captions:
+                combined_captions[start_time]["text"] += " " + text
+            else:
+                combined_captions[start_time] = {
+                    "time": start_time,
+                    "text": text,
+                }
+
+    return list(combined_captions.values())
 
 
-def read_sub(path) -> List[str]:
+def read_sub(path):
     if Path(path).suffix.lower() != ".srt":
         path = convert_to_srt(path)
 
     try:
         return read_sub_unsafe(path)
     except UnicodeDecodeError:
         return read_sub_unsafe(convert_to_srt(path))
 
 
-def subs_to_text(video_path, paths: List[str]) -> str:
-    def sub_to_text(path):
-        try:
-            return read_sub(path)
-        except UnicodeDecodeError:
-            log.warning(f"[{video_path}] Could not decode subtitle {path}")
-            return []
-
-    subtitles = " ".join(list(dict.fromkeys(flatten([sub_to_text(path) for path in paths]))))
-    return remove_consecutive_whitespace(subtitles)
-
-
 def is_text_subtitle_stream(s) -> bool:
     return s.get("codec_type") == "subtitle" and s.get("codec_name") not in IMAGE_SUBTITLE_CODECS
 
 
-def externalize_internal_subtitles(f, streams=None) -> List[str]:
+def externalize_internal_subtitles(path, streams=None) -> List[str]:
     if streams is None:
-        streams = ffmpeg.probe(f, show_chapters=None)["streams"]
+        streams = ffmpeg.probe(path, show_chapters=None)["streams"]
 
     external_paths = utils.conform(
-        [extract(f, s["index"]) for s in streams if is_text_subtitle_stream(s)],
+        [extract_from_video(path, s["index"]) for s in streams if is_text_subtitle_stream(s)],
     )
 
     return external_paths
 
 
 def get_external(file) -> List[str]:
     p = Path(file)
@@ -99,25 +117,25 @@
 
     if subtitles:
         return subtitles
 
     return []
 
 
-def get_subtitle_paths(f) -> List[str]:
-    internal_subtitles = externalize_internal_subtitles(f)
+def get_subtitle_paths(path) -> List[str]:
+    internal_subtitles = externalize_internal_subtitles(path)
     if len(internal_subtitles) > 0:
         return internal_subtitles
 
-    external_subtitles = get_external(f)
+    external_subtitles = get_external(path)
     return external_subtitles
 
 
-def get_sub_index(args, f) -> Optional[int]:
-    streams = ffmpeg.probe(f)["streams"]
+def get_sub_index(args, path) -> Optional[int]:
+    streams = ffmpeg.probe(path)["streams"]
     temp_db = db.connect(args, memory=True)
     temp_db["streams"].insert_all(streams, pk="index")  # type: ignore
     subtitle_index = temp_db.pop(
         f"""select "index" from streams
             where codec_type = "subtitle"
               and codec_name not in ({",".join(['?'] * len(IMAGE_SUBTITLE_CODECS))})
             order by
```

### Comparing `xklb-1.28.9/xklb/tabs_actions.py` & `xklb-1.29.1/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/tabs_extract.py` & `xklb-1.29.1/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/tube_backend.py` & `xklb-1.29.1/xklb/tube_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse, json, sys
 from copy import deepcopy
 from datetime import datetime, timezone
 from pathlib import Path
 from types import ModuleType
 from typing import Dict, List, Optional, Tuple
 
-from xklb import consts, fs_extract, utils
+from xklb import consts, fs_extract, subtitle, utils
 from xklb.consts import DBType
 from xklb.dl_config import (
     prefix_unrecoverable_errors,
     yt_meaningless_errors,
     yt_recoverable_errors,
     yt_unrecoverable_errors,
 )
@@ -218,14 +218,15 @@
     cv["time_played"] = 0
     cv["playhead"] = 0
     language = v.pop("language", None)
     cv["tags"] = combine(
         "language:" + language if language else None,
         v.pop("description", None),
         v.pop("categories", None),
+        v.pop("genre", None),
         v.pop("tags", None),
     )
     cv["id"] = v.pop("id", None)
     if cv["id"] is None:
         log.warning("No id found in %s", v)
     cv["ie_key"] = safe_unpack(v.pop("ie_key", None), v.pop("extractor_key", None), v.pop("extractor", None))
     cv["title"] = safe_unpack(v.pop("title", None), v.get("playlist_title"))
@@ -369,21 +370,26 @@
     m_columns = args.db["media"].columns_dict
 
     with yt_dlp.YoutubeDL(
         tube_opts(
             args,
             func_opts={
                 "subtitlesformat": "srt/best",
-                "writesubtitles": True,
-                "writeautomaticsub": True,
-                "subtitleslangs": ["en.*", "EN.*"],
+                "writesubtitles": args.subs,
+                "writeautomaticsub": args.auto_subs,
+                "subtitleslangs": args.subtitle_languages,
                 "extract_flat": False,
                 "lazy_playlist": False,
-                "skip_download": True,
                 "check_formats": False,
+                "skip_download": True,
+                "outtmpl": {
+                    "default": str(
+                        Path(f"{consts.SUB_TEMP_DIR}/%(uploader,uploader_id)s/%(title).200B_[%(id).60B].%(ext)s")
+                    ),
+                },
                 "ignoreerrors": True,
             },
             playlist_opts=playlist_dl_opts,
         ),
     ) as ydl:
         videos = args.db.execute(
             f"""
@@ -401,24 +407,50 @@
             ORDER by random()
             """,
             [playlist_path],
         ).fetchall()
 
         current_video_count = 0
         for path, ie_key, play_count, time_played, playhead in videos:
-            entry = ydl.extract_info(path, ie_key=ie_key, download=False)
+            entry = ydl.extract_info(path, ie_key=ie_key)
             if entry is None:
                 continue
 
+            chapters = getattr(entry, "chapters", [])
+            chapter_count = len(chapters)
+            if chapter_count > 0:
+                chapters = [
+                    {"path": path, "time": int(float(d["start_time"])), "text": d.get("title")}
+                    for d in chapters
+                    if d.get("title") and not utils.is_generic_title(d)
+                ]
+                if len(chapters) > 0:
+                    args.db["captions"].insert_all(chapters, alter=True)
+
+            if entry["requested_subtitles"]:
+                downloaded_subtitles = [d["filepath"] for d in entry["requested_subtitles"].values()]
+
+                captions = []
+                for subtitle_path in downloaded_subtitles:
+                    try:
+                        file_captions = subtitle.read_sub(subtitle_path)
+                    except UnicodeDecodeError:
+                        log.warning(f"[{path}] Could not decode subtitle {subtitle_path}")
+                    else:
+                        captions.extend([{"path": path, **d} for d in file_captions])
+                if len(captions) > 0:
+                    args.db["captions"].insert_all(captions, alter=True)
+
             entry = consolidate(entry)
             if entry is None:
                 continue
 
             entry["playlist_path"] = playlist_path
             entry["play_count"] = play_count
+            entry["chapter_count"] = chapter_count
             entry["time_played"] = time_played
             entry["playhead"] = playhead
             args.db["media"].upsert(utils.dict_filter_bool(entry), pk="path", alter=True)
 
             current_video_count += 1
             sys.stdout.write("\033[K\r")
             print(
@@ -463,16 +495,16 @@
     if Path(info["local_path"]).exists():
         fs_args = argparse.Namespace(
             profile=args.profile,
             scan_subtitles=args.profile == DBType.video,
             ocr=False,
             speech_recognition=False,
             delete_unplayable=False,
-            check_corrupt=False,
-            delete_corrupt=False,
+            check_corrupt=0.0,
+            delete_corrupt=None,
         )
         fs_tags = utils.dict_filter_bool(fs_extract.extract_metadata(fs_args, info["local_path"]), keep_0=False) or {}
         fs_extract.clean_up_temp_dirs()
     else:
         fs_tags = {}
 
     tube_entry = consolidate(info) or {}
@@ -547,17 +579,17 @@
                 "%(uploader,uploader_id)s/%(title).200B_%(section_number)03d_%(section_title)s_[%(id).60B].%(ext)s",
             ),
         },
     }
 
     if args.profile != DBType.audio:
         func_opts["subtitlesformat"] = "srt/best"
-        func_opts["subtitleslangs"] = ["en.*", "EN.*"]
-        func_opts["writesubtitles"] = True
-        func_opts["writeautomaticsub"] = True
+        func_opts["subtitleslangs"] = args.subtitle_languages
+        func_opts["writesubtitles"] = args.subs
+        func_opts["writeautomaticsub"] = args.auto_subs
         func_opts["postprocessors"].append({"key": "FFmpegEmbedSubtitle"})
 
     ydl_opts = tube_opts(
         args,
         func_opts=func_opts,
         playlist_opts=m.get("dl_config", "{}"),
     )
```

### Comparing `xklb-1.28.9/xklb/tube_extract.py` & `xklb-1.29.1/xklb/tube_extract.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,21 +24,25 @@
     )
     parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
     parser.add_argument("--extra", "-extra", action="store_true", help="Get full metadata (takes a lot longer)")
     parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
     parser.add_argument("--playlist-db", action="store_true", help="Fetch metadata for paths in a table")
+    parser.add_argument("--subs", action="store_true")
+    parser.add_argument("--auto-subs", "--autosubs", action="store_true")
+    parser.add_argument("--subtitle-languages", "--subtitle-language", "--slang", "--lang", action="extend", nargs="+")
     parser.add_argument("--extra-media-data", default={})
     parser.add_argument("--extra-playlist-data", default={})
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", "-f", action="store_true", help=argparse.SUPPRESS)
 
     if action in (SC.tubeadd, SC.tubeupdate):
         parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
 
+    parser.add_argument("--timeout", "-T", help="Quit after x minutes")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     if action == SC.tubeadd:
         parser.add_argument("playlists", nargs="+", help=argparse.SUPPRESS)
 
@@ -53,14 +57,16 @@
 
     if hasattr(args, "no_sanitize") and hasattr(args, "playlists") and not args.no_sanitize:
         args.playlists = [utils.sanitize_url(args, p) for p in args.playlists]
     if hasattr(args, "playlists"):
         args.playlists = utils.conform(args.playlists)
     log.info(utils.dict_filter_bool(args.__dict__))
 
+    utils.timeout(args.timeout)
+
     return args
 
 
 def tube_add(args=None) -> None:
     if args:
         sys.argv = ["tubeadd", *args]
 
@@ -129,15 +135,15 @@
 
         tube_backend.process_playlist(args, path, tube_backend.tube_opts(args))
 
         if args.extra:
             log.warning("[%s]: Getting extra metadata", path)
             tube_backend.get_extra_metadata(args, path)
 
-    LARGE_NUMBER = 100000
+    LARGE_NUMBER = 100_000
     if not args.db["media"].detect_fts() or tube_backend.added_media_count > LARGE_NUMBER:
         db.optimize(args)
 
 
 def tube_update(args=None) -> None:
     if args:
         sys.argv = ["tubeupdate", *args]
```

### Comparing `xklb-1.28.9/xklb/utils.py` & `xklb-1.29.1/xklb/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-import argparse, enum, functools, hashlib, logging, math, multiprocessing, os, platform, random, re, shlex, shutil, signal, string, subprocess, sys, tempfile, textwrap, time
+import argparse, csv, enum, functools, hashlib, logging, math, multiprocessing, os, platform, random, re, shlex, shutil, signal, string, subprocess, sys, tempfile, textwrap, time
 from ast import literal_eval
 from collections.abc import Iterable
 from datetime import datetime, timedelta, timezone
 from functools import wraps
 from pathlib import Path
 from random import shuffle
 from shutil import which
 from timeit import default_timer
 from typing import Any, Dict, Generator, List, NoReturn, Optional, Union
 
-import humanize
+import ffmpeg, humanize
 from IPython.core import ultratb
 from IPython.terminal.debugger import TerminalPdb
 from rich import prompt
 from rich.logging import RichHandler
 
-from xklb import consts, data
+from xklb import consts
+from xklb.scripts.mining import data
 
 try:
     import ipdb
 except ModuleNotFoundError:
     pass
 else:
     sys.breakpointhook = ipdb.set_trace
@@ -48,16 +49,16 @@
         if args.verbose > 0 and os.getpgrp() == os.tcgetpgrp(sys.stdout.fileno()):
             sys.excepthook = ultratb.FormattedTB(
                 mode="Context",
                 color_scheme="Neutral",
                 call_pdb=True,
                 debugger_cls=TerminalPdb,
             )
-    except Exception as e:
-        log.debug(e)
+    except Exception:
+        pass
 
     log_levels = [logging.WARNING, logging.INFO, logging.DEBUG]
     logging.root.handlers = []  # clear any existing handlers
     logging.basicConfig(
         level=log_levels[min(len(log_levels) - 1, args.verbose)],
         format="%(message)s",
         handlers=[RichHandler(show_time=False, show_level=False, show_path=False)],
@@ -268,26 +269,26 @@
         shutil.copyfileobj(fo_src, fo_dest)
     fo_dest.seek(0)
     fname = fo_dest.name
     fo_dest.close()
     return fname
 
 
-def trash(f: Union[Path, str], detach=True) -> None:
+def trash(path: Union[Path, str], detach=True) -> None:
     trash_put = which("trash-put") or which("trash")
     if trash_put is not None:
         if not detach:
-            cmd(trash_put, f, strict=False)
+            cmd(trash_put, path, strict=False)
             return
         try:
-            cmd_detach(trash_put, f)
+            cmd_detach(trash_put, path)
         except Exception:
-            cmd(trash_put, f, strict=False)
+            cmd(trash_put, path, strict=False)
     else:
-        Path(f).unlink(missing_ok=True)
+        Path(path).unlink(missing_ok=True)
 
 
 def remove_consecutive_whitespace(s) -> str:
     return " ".join(s.split())  # spaces, tabs, and newlines
 
 
 def remove_consecutive(s, char=" ") -> str:
@@ -345,14 +346,30 @@
         .replace(" _", "_")
         .replace("_ ", "_")
     )
     p = remove_consecutive_whitespace(p)
     return p
 
 
+def path_to_sentence(s):
+    return remove_consecutive_whitespace(
+        s.replace("/", " ")
+        .replace("\\", " ")
+        .replace(".", " ")
+        .replace("[", " ")
+        .replace("(", " ")
+        .replace("]", " ")
+        .replace(")", " ")
+        .replace("{", " ")
+        .replace("}", " ")
+        .replace("_", " ")
+        .replace("-", " ")
+    )
+
+
 def safe_int(s) -> Optional[int]:
     try:
         return int(float(s))
     except Exception:
         return None
 
 
@@ -361,19 +378,15 @@
         return None
 
     cleaned_string = re.sub(r"[^\w\s]", " ", string)
     words = [remove_consecutive_whitespace(s) for s in cleaned_string.split()]
     words = [
         s
         for s in words
-        if not (
-            s.lower() in data.stop_words
-            or s.lower() in data.prepositions
-            or (safe_int(s) is not None and safe_int(s) < 100)
-        )
+        if not (s.lower() in data.stop_words or s.lower() in data.prepositions or safe_int(s) is not None)
     ]
     return words
 
 
 def clean_path(b, dot_space=False) -> str:
     import ftfy
 
@@ -495,15 +508,15 @@
             "time_partial_first": int(p.stat().st_ctime),
             "time_partial_last": int(p.stat().st_mtime),
             "progress": safe_int(mpv_watchlater_value(p, "start")),
         }
         for p in paths
         if md5s.get(p.stem)
     ]
-    if "s" in args.partial:  # only unseen
+    if "s" in args.partial:  # skip; only play unseen
         previously_watched_paths = [m["path"] for m in previously_watched]
         return [m for m in media if m["path"] not in previously_watched_paths]
 
     def mpv_progress(m):
         progress = m.get("progress")
         duration = m.get("duration")
         if not progress:
@@ -674,16 +687,36 @@
     return humanize.precisedelta(timedelta(seconds=int(seconds)), minimum_unit="minutes")
 
 
 def col_duration(tbl: List[Dict], col: str) -> List[Dict]:
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
             tbl[idx][col] = human_time(tbl[idx][col])
+    return tbl
 
-    col_resize(tbl, "duration", 6)
+
+def seconds_to_hhmmss(seconds):
+    if seconds < 0:
+        seconds = abs(seconds)
+
+    hours = seconds // 3600
+    minutes = (seconds % 3600) // 60
+    seconds = seconds % 60
+
+    formatted_time = f"{hours:02d}:{minutes:02d}:{seconds:02d}"
+    if hours == 0:
+        formatted_time = f"   {minutes:02d}:{seconds:02d}"
+
+    return formatted_time
+
+
+def col_hhmmss(tbl: List[Dict], col: str) -> List[Dict]:
+    for idx, _d in enumerate(tbl):
+        if tbl[idx].get(col) is not None:
+            tbl[idx][col] = seconds_to_hhmmss(tbl[idx][col])
     return tbl
 
 
 class ArgparseDict(argparse.Action):
     def __call__(self, parser, args, values, option_string=None):
         try:
             d = {}
@@ -980,7 +1013,148 @@
     def elapsed(self):
         if not hasattr(self, "start_time"):
             raise RuntimeError("Timer has not been started.")
         end_time = default_timer()
         elapsed_time = end_time - self.start_time
         self.reset()
         return elapsed_time
+
+
+def cover_scan(media_duration, scan_percentage):
+    num_scans = max(2, int(math.log(media_duration) * (scan_percentage / 10)))
+    scan_duration_total = max(1, media_duration * (scan_percentage / 100))
+    scan_duration = max(1, int(scan_duration_total / num_scans))
+    scan_interval = media_duration / num_scans
+
+    scans = sorted(set(int(scan * scan_interval) for scan in range(num_scans)))
+    if scans[-1] < media_duration - (scan_duration * 2):
+        scans.append(math.floor(media_duration - scan_duration))
+
+    return scans, scan_duration
+
+
+def decode_full_scan(path):
+    output = ffmpeg.input(path).output("/dev/null", f="null")
+    error_log = ffmpeg.run(output, quiet=True)
+
+
+def decode_quick_scan(path, scans, scan_duration=3):
+    fail_count = 0
+    for scan in scans:
+        try:
+            output = ffmpeg.input(path, ss=scan).output("/dev/null", t=scan_duration, f="null")
+            error_log = ffmpeg.run(output, quiet=True)
+        except ffmpeg.Error:
+            fail_count += 1
+
+    return (fail_count / len(scans)) * 100
+
+
+def fast_glob(path_dir, limit=100):
+    files = []
+    with os.scandir(path_dir) as entries:
+        for entry in entries:
+            if entry.is_file():
+                files.append(entry.path)
+                if len(files) == limit:
+                    break
+    return sorted(files)
+
+
+def load_spacy_model(model=None):
+    try:
+        import spacy
+    except ModuleNotFoundError:
+        log.error("Install spaCy and sklearn to use:")
+        log.error("pip install spacy sklearn")
+        log.error("python -m spacy download en_core_web_sm")
+        exit(1)
+
+    if model:
+        return spacy.load(model)
+
+    model_sizes = ["lg", "md", "sm"]
+    loaded_model = None
+
+    for size in model_sizes:
+        try:
+            loaded_model = spacy.load(f"en_core_web_{size}")
+            log.info(f"Loaded 'en_core_web_{size}'")
+        except OSError:
+            pass
+
+    if loaded_model:
+        return loaded_model
+
+    log.error("Language model not found. Download a model first using the following commands:")
+    log.error("python -m spacy download en_core_web_sm")
+    exit(1)
+
+
+def cluster_paths(paths, model=None, n_clusters=None):
+    nlp = load_spacy_model(model)
+
+    from sklearn.cluster import KMeans
+    from sklearn.feature_extraction.text import TfidfVectorizer
+
+    sentence_strings = (path_to_sentence(s) for s in paths)
+
+    joined_strings = []
+    for doc in nlp.pipe(sentence_strings, n_process=4):
+        joined_strings.append(" ".join([token.lower_ for token in doc if not token.is_stop]))
+
+    vectorizer = TfidfVectorizer()
+    X = vectorizer.fit_transform(joined_strings)
+
+    kmeans = KMeans(n_clusters=n_clusters or int(X.shape[0] ** 0.5), random_state=0).fit(X)
+    clusters = kmeans.labels_
+
+    grouped_strings = {}
+    for i, string in enumerate(paths):
+        cluster_id = clusters[i]
+
+        if cluster_id not in grouped_strings:
+            grouped_strings[cluster_id] = []
+
+        grouped_strings[cluster_id].append(string)
+
+    result = []
+    for _cluster_id, paths in grouped_strings.items():
+        common_prefix = os.path.commonprefix(paths)
+        metadata = {
+            "common_prefix": common_prefix,
+            "grouped_paths": sorted(paths),
+        }
+        result.append(metadata)
+
+    return result
+
+
+def is_timecode_like(text):
+    for char in text:
+        if not (char in ":,_-;. " or char.isdigit()):
+            return False
+    return True
+
+
+def is_generic_title(title):
+    return (
+        (len(title) <= 12 and (title.startswith("Chapter") or title.startswith("Scene")))
+        or "Untitled Chapter" in title
+        or is_timecode_like(title)
+        or title.isdigit()
+    )
+
+
+def write_csv_to_stdout(data):
+    fieldnames = data[0].keys()
+    writer = csv.DictWriter(sys.stdout, fieldnames=fieldnames)
+    writer.writeheader()
+    writer.writerows(data)
+
+
+def order_set(items):
+    seen = set()
+    for item in items:
+        if item not in seen:
+            yield item
+            seen.add(item)
```

### Comparing `xklb-1.28.9/xklb/scripts/bigdirs.py` & `xklb-1.29.1/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/christen.py` & `xklb-1.29.1/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/copy_play_counts.py` & `xklb-1.29.1/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/dedupe.py` & `xklb-1.29.1/xklb/scripts/dedupe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, operator, tempfile
+import argparse, tempfile
 from copy import deepcopy
 from pathlib import Path
 from typing import List
 
 import humanize
 from tabulate import tabulate
 
@@ -255,15 +255,15 @@
 
         csv_path = tempfile.mktemp(".csv")
         pd.DataFrame(duplicates).to_csv(csv_path, index=False)
         print("Full list saved to:", csv_path)
     except ModuleNotFoundError:
         log.info("Skipping CSV export because pandas is not installed")
 
-    duplicates_size = sum(filter(None, map(operator.itemgetter("duplicate_size"), duplicates)))
+    duplicates_size = sum(filter(None, [d["duplicate_size"] for d in duplicates]))
     print(f"Approx. space savings: {humanize.naturalsize(duplicates_size // 2)}")
 
     if duplicates and (args.force or utils.confirm("Delete duplicates?")):  # type: ignore
         log.info("Deleting...")
         for d in duplicates:
             path = d["duplicate_path"]
             if not path.startswith("http") and not args.only_soft_delete:
```

### Comparing `xklb-1.28.9/xklb/scripts/merge_dbs.py` & `xklb-1.29.1/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/merge_online_local.py` & `xklb-1.29.1/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/move_list.py` & `xklb-1.29.1/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/optimize_db.py` & `xklb-1.29.1/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/redownload.py` & `xklb-1.29.1/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/relmv.py` & `xklb-1.29.1/xklb/scripts/relmv.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library relmv",
         usage="""library relmv [--dry-run] SOURCE ... DEST
 
     Move files/folders without losing hierarchy metadata
+
+    Move fresh music to your phone every Sunday:
+
+        # move last weeks' music back to their source folders
+        lb relmv /mnt/d/80_Now_Listening/ /mnt/d/
+
+        # move new music for this week
+        lb relmv (
+            lb listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
+        ) /mnt/d/80_Now_Listening/
 """,
     )
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--test", "--dry-run", action="store_true")
 
     parser.add_argument("sources", nargs="+", help="one or more source files or directories to move")
     parser.add_argument("dest", help="destination directory")
```

### Comparing `xklb-1.28.9/xklb/scripts/scatter.py` & `xklb-1.29.1/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/streaming_tab_loader.py` & `xklb-1.29.1/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/mining/extract_links.py` & `xklb-1.29.1/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/mining/nouns.py` & `xklb-1.29.1/xklb/scripts/mining/nouns.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 from html.parser import HTMLParser
 from io import StringIO
 
-from xklb import data
+from xklb.scripts.mining import data
 from xklb.utils import pipe_print
 
 """
 extract compound nouns and phrases from unstructured mixed HTML plain text
 
 xsv select text hn_comment_202210242109.csv | library nouns | sort | uniq -c | sort --numeric-sort
 """
```

### Comparing `xklb-1.28.9/xklb/scripts/mining/pushshift.py` & `xklb-1.29.1/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.29.1/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/.gitignore` & `xklb-1.29.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/LICENSE` & `xklb-1.29.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.28.9/README.md` & `xklb-1.29.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,107 +1,32 @@
 # xk media library
 
-A wise philosopher once told me: "[the future is autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
+A wise philosopher once told me: "the future is [autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
-Manage large media libraries. An index for your archive.
+Manage and curate large media libraries. An index for your archive.
 Primary usage is local filesystem but also supports some virtual constructs like
 tracking online video playlists (eg. YouTube subscriptions) and scheduling browser tabs.
 
-Required: `ffmpeg`
-
-Recommended: `mpv`, `fish`, `firefox`
-
 ## Install
 
 Linux recommended but [Windows setup instructions](./Windows.md) available.
 
     pip install xklb
 
-## Examples
-
-<details><summary>List all subcommands</summary>
-
-    $ library
-    xk media library subcommands (v1.28.009)
-
-    local media:
-      lb fsadd                 Create a local media database; Add folders
-      lb fsupdate              Refresh database: add new files, mark deleted
-
-      lb listen                Listen to local and online media
-      lb watch                 Watch local and online media
-      lb read                  Read books
-      lb view                  View images
-
-      lb bigdirs               Discover folders which take much room
-      lb dedupe                Deduplicate local db files
-      lb relmv                 Move files/folders while preserving relative paths
-      lb christen              Cleanse files by giving them a new name
-
-      lb mv-list               Reach a target free space by moving data across mount points
-      lb scatter               Scatter files across multiple mountpoints (mergerfs balance)
-
-      lb merge-dbs             Merge multiple SQLITE files
-      lb copy-play-counts      Copy play counts from multiple SQLITE files
-
-    online media:
-      lb tubeadd               Create a tube database; Add playlists
-      lb tubeupdate            Fetch new videos from saved playlists
-
-      lb redditadd             Create a reddit database; Add subreddits
-      lb redditupdate          Fetch new posts from saved subreddits
-
-    downloads:
-      lb download              Download media
-      lb redownload            Redownload missing media
-      lb block                 Prevent downloading specific URLs
-      lb merge-online-local    Merge local and online metadata
-
-    playback:
-      lb now                   Print what is currently playing
-      lb next                  Play next file
-      lb stop                  Stop all playback
-      lb pause                 Pause all playback
-
-    statistics:
-      lb playlists             List added playlists
-      lb dlstatus              Show download status
-      lb usage                 Print mount usage
-
-    browser tabs:
-      lb tabsadd               Create a tabs database; Add URLs
-      lb tabs                  Open your tabs for the day
-      lb surf                  Load browser tabs in a streaming way (stdin)
-
-    mining:
-      lb extract-links         Extract links from lists of web pages
-      lb reddit-selftext       db selftext external links -> db media table
-      lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
-      lb nouns                 Unstructured text -> compound nouns (stdin)
-      lb hnadd                 Create a hackernews database (this takes a few days)
-    
-
-</details>
+Should also work on Mac OS.
 
-### Watch online media on your PC
+### External dependencies
 
-    wget https://github.com/chapmanjacobd/library/raw/main/examples/mealtime.tw.db
-    library watch mealtime.tw.db
+Required: `ffmpeg`
 
-### Listen to online media on a chromecast group
+Some features work better with: `mpv`, `firefox`, `fish`
 
-    wget https://github.com/chapmanjacobd/library/raw/main/examples/music.tl.db
-    library listen music.tl.db -ct "House speakers"
+## Getting started
 
-### Hook into HackerNews
-
-    wget https://github.com/chapmanjacobd/hn_mining/raw/main/hackernews_only_direct.tw.db
-    library watch hackernews_only_direct.tw.db --random --ignore-errors
-
-## Getting started with local media
+<details><summary>Local media</summary>
 
 ### 1. Extract Metadata
 
 For thirty terabytes of video the initial scan takes about four hours to complete.
 After that, subsequent scans of the path (or any subpaths) are much quicker--only
 new files will be read by `ffprobe`.
 
@@ -113,15 +38,17 @@
 
     library watch tv.db                           # the default post-action is to do nothing
     library watch tv.db --post-action delete      # delete file after playing
     library listen finalists.db -k ask_keep       # ask whether to keep file after playing
 
 To stop playing press Ctrl+C in either the terminal or mpv
 
-## Getting started with online media
+</details>
+
+<details><summary>Online media</summary>
 
 ### 1. Download Metadata
 
 Download playlist and channel metadata. Break free of the YouTube algo~
 
     library tubeadd educational.db https://www.youtube.com/c/BranchEducation/videos
 
@@ -203,15 +130,103 @@
     systemctl --user daemon-reload
     systemctl --user enable --now tabs.service
 
 You can also invoke tabs manually:
 
     library tabs tabs.db -L 1  # open one tab
 
-## Usage
+</details>
+
+<details><summary>List all subcommands</summary>
+
+    $ library
+    xk media library subcommands (v1.29.001)
+
+    local media:
+      lb fsadd                 Create a local media database; Add folders
+      lb fsupdate              Refresh database: add new files, mark deleted
+
+      lb listen                Listen to local and online media
+      lb watch                 Watch local and online media
+      lb search                Search text and subtitles
+
+      lb read                  Read books
+      lb view                  View images
+
+      lb bigdirs               Discover folders which take much room
+      lb dedupe                Deduplicate local db files
+      lb relmv                 Move files/folders while preserving relative paths
+      lb christen              Cleanse files by giving them a new name
+
+      lb mv-list               Reach a target free space by moving data across mount points
+      lb scatter               Scatter files across multiple mountpoints (mergerfs balance)
+
+      lb merge-dbs             Merge multiple SQLITE files
+      lb copy-play-counts      Copy play counts from multiple SQLITE files
+
+    online media:
+      lb tubeadd               Create a tube database; Add playlists
+      lb tubeupdate            Fetch new videos from saved playlists
+
+      lb redditadd             Create a reddit database; Add subreddits
+      lb redditupdate          Fetch new posts from saved subreddits
+
+    downloads:
+      lb download              Download media
+      lb redownload            Redownload missing media
+      lb block                 Prevent downloading specific URLs
+      lb merge-online-local    Merge local and online metadata
+
+    playback:
+      lb now                   Print what is currently playing
+      lb next                  Play next file
+      lb stop                  Stop all playback
+      lb pause                 Pause all playback
+
+    statistics:
+      lb playlists             List added playlists
+      lb dlstatus              Show download status
+      lb usage                 Print mount usage
+
+    browser tabs:
+      lb tabsadd               Create a tabs database; Add URLs
+      lb tabs                  Open your tabs for the day
+      lb surf                  Load browser tabs in a streaming way (stdin)
+
+    mining:
+      lb reddit-selftext       db selftext external links -> db media table
+      lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
+      lb hnadd                 Create a hackernews database (this takes a few days)
+
+      lb extract-links         Extract links from lists of web pages
+
+      lb cluster-sort          Lines -> sorted by sentence similarity groups (stdin)
+      lb nouns                 Unstructured text -> compound nouns (stdin)
+    
+
+</details>
+
+## Examples
+
+### Watch online media on your PC
+
+    wget https://github.com/chapmanjacobd/library/raw/main/examples/mealtime.tw.db
+    library watch mealtime.tw.db
+
+### Listen to online media on a chromecast group
+
+    wget https://github.com/chapmanjacobd/library/raw/main/examples/music.tl.db
+    library listen music.tl.db -ct "House speakers"
+
+### Hook into HackerNews
+
+    wget https://github.com/chapmanjacobd/hn_mining/raw/main/hackernews_only_direct.tw.db
+    library watch hackernews_only_direct.tw.db --random --ignore-errors
+
+## Watch/Listen Usage
 
     $ library watch -h
     usage: library watch [database] [optional args]
 
     Control playback:
         To stop playback press Ctrl-C in either the terminal or mpv
 
@@ -227,22 +242,29 @@
         library watch --cast --cast-to "Office pair"
         library watch -ct "Office pair"  # equivalent
         If you don't know the exact name of your chromecast group run `catt scan`
 
     Play media in order (similarly named episodes):
         library watch --play-in-order
         There are multiple strictness levels of --play-in-order:
-        library watch -O   # equivalent
-        library watch -OO  # above, plus ignores most filters
-        library watch -OOO # above, plus ignores include/exclude filter during ordinal search
+        library watch -O    # equivalent
+        library watch -OO   # above, plus ignores most filters
+        library watch -OOO  # above, plus ignores fts and (include/exclude) filter during ordinal search
+        library watch -OOOO # above, plus starts search with parent folder
 
         library watch --related  # similar to -O but uses fts to find similar content
         library watch -R         # equivalent
         library watch -RR        # above, plus ignores most filters
 
+        library watch --cluster  # cluster-sort to put similar paths closer together
+
+        All of these options can be used together but it will be a bit slow and the results might be mid-tier
+        as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
+        library watch -RRCOO
+
     Filter media by file siblings of parent directory:
         library watch --sibling   # only include files which have more than or equal to one sibling
         library watch --solo      # only include files which are alone by themselves
 
         `--sibling` is just a shortcut for `--lower 2`; `--solo` is `--upper 1`
         library watch --sibling --solo      # you will always get zero records here
         library watch --lower 2 --upper 1   # equivalent
@@ -463,15 +485,35 @@
 
 ### Organize via separate databases.
 
     library fsadd --audio both.db ./audiobooks/ ./podcasts/
     library fsadd --audio audiobooks.db ./audiobooks/
     library fsadd --audio podcasts.db ./podcasts/ ./another/more/secret/podcasts_folder/
 
-### Find large folders to curate or candidates for freeing up space by moving to another mount point
+
+### Find large folders to curate
+
+<details><summary>lb bigdirs</summary>
+
+Also, if you are just looking for folders which are candidates for curation (ie. I need space but don't want to buy a hard drive). The bigdirs subcommand was written for that purpose:
+
+    $ lb bigdirs fs/d.db
+
+You may filter by folder depth (similar to QDirStat or WizTree)
+
+    $ lb bigdirs --depth=3 audio.db
+
+There is also an flag to prioritize folders which have many files which have been deleted (for example you delete songs you don't like--now you can see who wrote those songs and delete all their other songs...)
+
+    $ lb bigdirs --sort-by deleted audio.db
+
+</details>
+
+
+### Find candidates for freeing up space by moving to another mount point
 
 <details><summary>lb mv-list</summary>
 
 The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
 
     $ lb fsadd --filesystem d.db ~/d/
 
@@ -523,30 +565,14 @@
 
         Folder list saved to /tmp/tmpa7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
 
             rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmpa7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
 
 </details>
 
-<details><summary>lb bigdirs</summary>
-
-Also, if you are just looking for folders which are candidates for curation (ie. I need space but don't want to buy a hard drive). The bigdirs subcommand was written for that purpose:
-
-    $ lb bigdirs fs/d.db
-
-You may filter by folder depth (similar to QDirStat or WizTree)
-
-    $ lb bigdirs --depth=3 audio.db
-
-There is also an flag to prioritize folders which have many files which have been deleted (for example you delete songs you don't like--now you can see who wrote those songs and delete all their other songs...)
-
-    $ lb bigdirs --sort-by deleted audio.db
-
-</details>
-
 
 ### Scatter your data across disks with [mergerfs](https://github.com/trapexit/mergerfs)
 
 <details><summary>If you use mergerfs, you'll likely be interested in this</summary>
 
     library scatter -h
     usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS database relative_paths ...
@@ -635,25 +661,27 @@
     pip install mnamer
     mnamer --movie-directory ~/d/70_Now_Watching/ --episode-directory ~/d/70_Now_Watching/ \
         --no-overwrite -b (library watch -p fd -s 'path : McCloud')
     library fsadd ~/d/70_Now_Watching/
 
 </details>
 
-### Wake up to your own music (via termux)
+### Music alarm clock (via termux crontab)
+
+Wake up to your own music
 
-    30 9 * * * lb listen ./audio.db
+    30 7 * * * lb listen ./audio.db
 
-### Wake up to your own music _only when you are not home_ (computer on local-only IP)
+Wake up to your own music _only when you are *not* home_ (computer on local-only IP)
 
-    30 9 * * * timeout 0.4 nc -z 192.168.1.12 22 || lb listen --random
+    30 7 * * * timeout 0.4 nc -z 192.168.1.12 22 || lb listen --random
 
-### Wake up to your own music on your Chromecast speaker group _only when you are home_
+Wake up to your own music on your Chromecast speaker group _only when you are home_
 
-    30 9 * * * ssh 192.168.1.12 lb listen --random --play-in-order --cast --cast-to "Bedroom pair"
+    30 7 * * * ssh 192.168.1.12 lb listen --cast --cast-to "Bedroom pair"
 
 ### Pipe to [lowcharts](https://github.com/juan-leon/lowcharts)
 
 <details><summary>$ lb watch -p f -col time_created | lowcharts timehist -w 80</summary>
 
     Matches: 445183.
     Each ∎ represents a count of 1896
@@ -686,17 +714,18 @@
 
 ![fps](https://user-images.githubusercontent.com/7908073/184738438-ee566a4b-2da0-4e6d-a4b3-9bfca036aa2a.png)
 
 </details>
 
 ### Pipe to rsync
 
-<details><summary>Copy or move files to your phone via syncthing</summary>
+<details><summary>Move files to your phone via syncthing</summary>
 
-I use rsync to move files instead of copy-on-write duplication because I want deletions to stick.
+I used to use rsync to move files because I want deletions to stick.
+I now use `lb relmv`. But this is still a good rsync example:
 
     function mrmusic
         rsync -a --remove-source-files --files-from=(
             library lt ~/lb/audio.db -s /mnt/d/80_Now_Listening/ -p f \
             --moved /mnt/d/80_Now_Listening/ /mnt/d/ | psub
         ) /mnt/d/80_Now_Listening/ /mnt/d/
```

### Comparing `xklb-1.28.9/pyproject.toml` & `xklb-1.29.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 license = {file = "LICENSE"}
 name = "xklb"
 readme = "README.md"
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 all = ["xklb[deluxe,dev,test]"]
-deluxe = ["textract", "PyExifTool", "aiohttp", "brotab", "orjson", "pandas"]
+deluxe = ["textract", "PyExifTool", "aiohttp", "brotab", "orjson", "pandas", "spacy", "sklearn"]
 dev = ["black", "ipdb", "isort", "scalene", "ssort"]
 test = ["ruff", "pytest"]
 
 [project.urls]
 documentation = "https://github.com/chapmanjacobd/library/wiki/Usage"
 homepage = "https://github.com/chapmanjacobd/library/"
 repository = "https://github.com/chapmanjacobd/library/"
```

### Comparing `xklb-1.28.9/PKG-INFO` & `xklb-1.29.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.28.9
+Version: 1.29.1
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -64,126 +64,53 @@
 Requires-Dist: xklb[deluxe,dev,test]; extra == 'all'
 Provides-Extra: deluxe
 Requires-Dist: aiohttp; extra == 'deluxe'
 Requires-Dist: brotab; extra == 'deluxe'
 Requires-Dist: orjson; extra == 'deluxe'
 Requires-Dist: pandas; extra == 'deluxe'
 Requires-Dist: pyexiftool; extra == 'deluxe'
+Requires-Dist: sklearn; extra == 'deluxe'
+Requires-Dist: spacy; extra == 'deluxe'
 Requires-Dist: textract; extra == 'deluxe'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipdb; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: scalene; extra == 'dev'
 Requires-Dist: ssort; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: ruff; extra == 'test'
 Description-Content-Type: text/markdown
 
 # xk media library
 
-A wise philosopher once told me: "[the future is autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
+A wise philosopher once told me: "the future is [autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
-Manage large media libraries. An index for your archive.
+Manage and curate large media libraries. An index for your archive.
 Primary usage is local filesystem but also supports some virtual constructs like
 tracking online video playlists (eg. YouTube subscriptions) and scheduling browser tabs.
 
-Required: `ffmpeg`
-
-Recommended: `mpv`, `fish`, `firefox`
-
 ## Install
 
 Linux recommended but [Windows setup instructions](./Windows.md) available.
 
     pip install xklb
 
-## Examples
-
-<details><summary>List all subcommands</summary>
-
-    $ library
-    xk media library subcommands (v1.28.009)
-
-    local media:
-      lb fsadd                 Create a local media database; Add folders
-      lb fsupdate              Refresh database: add new files, mark deleted
-
-      lb listen                Listen to local and online media
-      lb watch                 Watch local and online media
-      lb read                  Read books
-      lb view                  View images
-
-      lb bigdirs               Discover folders which take much room
-      lb dedupe                Deduplicate local db files
-      lb relmv                 Move files/folders while preserving relative paths
-      lb christen              Cleanse files by giving them a new name
-
-      lb mv-list               Reach a target free space by moving data across mount points
-      lb scatter               Scatter files across multiple mountpoints (mergerfs balance)
-
-      lb merge-dbs             Merge multiple SQLITE files
-      lb copy-play-counts      Copy play counts from multiple SQLITE files
-
-    online media:
-      lb tubeadd               Create a tube database; Add playlists
-      lb tubeupdate            Fetch new videos from saved playlists
-
-      lb redditadd             Create a reddit database; Add subreddits
-      lb redditupdate          Fetch new posts from saved subreddits
-
-    downloads:
-      lb download              Download media
-      lb redownload            Redownload missing media
-      lb block                 Prevent downloading specific URLs
-      lb merge-online-local    Merge local and online metadata
-
-    playback:
-      lb now                   Print what is currently playing
-      lb next                  Play next file
-      lb stop                  Stop all playback
-      lb pause                 Pause all playback
-
-    statistics:
-      lb playlists             List added playlists
-      lb dlstatus              Show download status
-      lb usage                 Print mount usage
-
-    browser tabs:
-      lb tabsadd               Create a tabs database; Add URLs
-      lb tabs                  Open your tabs for the day
-      lb surf                  Load browser tabs in a streaming way (stdin)
-
-    mining:
-      lb extract-links         Extract links from lists of web pages
-      lb reddit-selftext       db selftext external links -> db media table
-      lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
-      lb nouns                 Unstructured text -> compound nouns (stdin)
-      lb hnadd                 Create a hackernews database (this takes a few days)
-    
-
-</details>
+Should also work on Mac OS.
 
-### Watch online media on your PC
+### External dependencies
 
-    wget https://github.com/chapmanjacobd/library/raw/main/examples/mealtime.tw.db
-    library watch mealtime.tw.db
+Required: `ffmpeg`
 
-### Listen to online media on a chromecast group
+Some features work better with: `mpv`, `firefox`, `fish`
 
-    wget https://github.com/chapmanjacobd/library/raw/main/examples/music.tl.db
-    library listen music.tl.db -ct "House speakers"
+## Getting started
 
-### Hook into HackerNews
-
-    wget https://github.com/chapmanjacobd/hn_mining/raw/main/hackernews_only_direct.tw.db
-    library watch hackernews_only_direct.tw.db --random --ignore-errors
-
-## Getting started with local media
+<details><summary>Local media</summary>
 
 ### 1. Extract Metadata
 
 For thirty terabytes of video the initial scan takes about four hours to complete.
 After that, subsequent scans of the path (or any subpaths) are much quicker--only
 new files will be read by `ffprobe`.
 
@@ -195,15 +122,17 @@
 
     library watch tv.db                           # the default post-action is to do nothing
     library watch tv.db --post-action delete      # delete file after playing
     library listen finalists.db -k ask_keep       # ask whether to keep file after playing
 
 To stop playing press Ctrl+C in either the terminal or mpv
 
-## Getting started with online media
+</details>
+
+<details><summary>Online media</summary>
 
 ### 1. Download Metadata
 
 Download playlist and channel metadata. Break free of the YouTube algo~
 
     library tubeadd educational.db https://www.youtube.com/c/BranchEducation/videos
 
@@ -285,15 +214,103 @@
     systemctl --user daemon-reload
     systemctl --user enable --now tabs.service
 
 You can also invoke tabs manually:
 
     library tabs tabs.db -L 1  # open one tab
 
-## Usage
+</details>
+
+<details><summary>List all subcommands</summary>
+
+    $ library
+    xk media library subcommands (v1.29.001)
+
+    local media:
+      lb fsadd                 Create a local media database; Add folders
+      lb fsupdate              Refresh database: add new files, mark deleted
+
+      lb listen                Listen to local and online media
+      lb watch                 Watch local and online media
+      lb search                Search text and subtitles
+
+      lb read                  Read books
+      lb view                  View images
+
+      lb bigdirs               Discover folders which take much room
+      lb dedupe                Deduplicate local db files
+      lb relmv                 Move files/folders while preserving relative paths
+      lb christen              Cleanse files by giving them a new name
+
+      lb mv-list               Reach a target free space by moving data across mount points
+      lb scatter               Scatter files across multiple mountpoints (mergerfs balance)
+
+      lb merge-dbs             Merge multiple SQLITE files
+      lb copy-play-counts      Copy play counts from multiple SQLITE files
+
+    online media:
+      lb tubeadd               Create a tube database; Add playlists
+      lb tubeupdate            Fetch new videos from saved playlists
+
+      lb redditadd             Create a reddit database; Add subreddits
+      lb redditupdate          Fetch new posts from saved subreddits
+
+    downloads:
+      lb download              Download media
+      lb redownload            Redownload missing media
+      lb block                 Prevent downloading specific URLs
+      lb merge-online-local    Merge local and online metadata
+
+    playback:
+      lb now                   Print what is currently playing
+      lb next                  Play next file
+      lb stop                  Stop all playback
+      lb pause                 Pause all playback
+
+    statistics:
+      lb playlists             List added playlists
+      lb dlstatus              Show download status
+      lb usage                 Print mount usage
+
+    browser tabs:
+      lb tabsadd               Create a tabs database; Add URLs
+      lb tabs                  Open your tabs for the day
+      lb surf                  Load browser tabs in a streaming way (stdin)
+
+    mining:
+      lb reddit-selftext       db selftext external links -> db media table
+      lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
+      lb hnadd                 Create a hackernews database (this takes a few days)
+
+      lb extract-links         Extract links from lists of web pages
+
+      lb cluster-sort          Lines -> sorted by sentence similarity groups (stdin)
+      lb nouns                 Unstructured text -> compound nouns (stdin)
+    
+
+</details>
+
+## Examples
+
+### Watch online media on your PC
+
+    wget https://github.com/chapmanjacobd/library/raw/main/examples/mealtime.tw.db
+    library watch mealtime.tw.db
+
+### Listen to online media on a chromecast group
+
+    wget https://github.com/chapmanjacobd/library/raw/main/examples/music.tl.db
+    library listen music.tl.db -ct "House speakers"
+
+### Hook into HackerNews
+
+    wget https://github.com/chapmanjacobd/hn_mining/raw/main/hackernews_only_direct.tw.db
+    library watch hackernews_only_direct.tw.db --random --ignore-errors
+
+## Watch/Listen Usage
 
     $ library watch -h
     usage: library watch [database] [optional args]
 
     Control playback:
         To stop playback press Ctrl-C in either the terminal or mpv
 
@@ -309,22 +326,29 @@
         library watch --cast --cast-to "Office pair"
         library watch -ct "Office pair"  # equivalent
         If you don't know the exact name of your chromecast group run `catt scan`
 
     Play media in order (similarly named episodes):
         library watch --play-in-order
         There are multiple strictness levels of --play-in-order:
-        library watch -O   # equivalent
-        library watch -OO  # above, plus ignores most filters
-        library watch -OOO # above, plus ignores include/exclude filter during ordinal search
+        library watch -O    # equivalent
+        library watch -OO   # above, plus ignores most filters
+        library watch -OOO  # above, plus ignores fts and (include/exclude) filter during ordinal search
+        library watch -OOOO # above, plus starts search with parent folder
 
         library watch --related  # similar to -O but uses fts to find similar content
         library watch -R         # equivalent
         library watch -RR        # above, plus ignores most filters
 
+        library watch --cluster  # cluster-sort to put similar paths closer together
+
+        All of these options can be used together but it will be a bit slow and the results might be mid-tier
+        as multiple different algorithms create a muddied signal (too many cooks in the kitchen):
+        library watch -RRCOO
+
     Filter media by file siblings of parent directory:
         library watch --sibling   # only include files which have more than or equal to one sibling
         library watch --solo      # only include files which are alone by themselves
 
         `--sibling` is just a shortcut for `--lower 2`; `--solo` is `--upper 1`
         library watch --sibling --solo      # you will always get zero records here
         library watch --lower 2 --upper 1   # equivalent
@@ -545,15 +569,35 @@
 
 ### Organize via separate databases.
 
     library fsadd --audio both.db ./audiobooks/ ./podcasts/
     library fsadd --audio audiobooks.db ./audiobooks/
     library fsadd --audio podcasts.db ./podcasts/ ./another/more/secret/podcasts_folder/
 
-### Find large folders to curate or candidates for freeing up space by moving to another mount point
+
+### Find large folders to curate
+
+<details><summary>lb bigdirs</summary>
+
+Also, if you are just looking for folders which are candidates for curation (ie. I need space but don't want to buy a hard drive). The bigdirs subcommand was written for that purpose:
+
+    $ lb bigdirs fs/d.db
+
+You may filter by folder depth (similar to QDirStat or WizTree)
+
+    $ lb bigdirs --depth=3 audio.db
+
+There is also an flag to prioritize folders which have many files which have been deleted (for example you delete songs you don't like--now you can see who wrote those songs and delete all their other songs...)
+
+    $ lb bigdirs --sort-by deleted audio.db
+
+</details>
+
+
+### Find candidates for freeing up space by moving to another mount point
 
 <details><summary>lb mv-list</summary>
 
 The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
 
     $ lb fsadd --filesystem d.db ~/d/
 
@@ -605,30 +649,14 @@
 
         Folder list saved to /tmp/tmpa7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
 
             rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmpa7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
 
 </details>
 
-<details><summary>lb bigdirs</summary>
-
-Also, if you are just looking for folders which are candidates for curation (ie. I need space but don't want to buy a hard drive). The bigdirs subcommand was written for that purpose:
-
-    $ lb bigdirs fs/d.db
-
-You may filter by folder depth (similar to QDirStat or WizTree)
-
-    $ lb bigdirs --depth=3 audio.db
-
-There is also an flag to prioritize folders which have many files which have been deleted (for example you delete songs you don't like--now you can see who wrote those songs and delete all their other songs...)
-
-    $ lb bigdirs --sort-by deleted audio.db
-
-</details>
-
 
 ### Scatter your data across disks with [mergerfs](https://github.com/trapexit/mergerfs)
 
 <details><summary>If you use mergerfs, you'll likely be interested in this</summary>
 
     library scatter -h
     usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS database relative_paths ...
@@ -717,25 +745,27 @@
     pip install mnamer
     mnamer --movie-directory ~/d/70_Now_Watching/ --episode-directory ~/d/70_Now_Watching/ \
         --no-overwrite -b (library watch -p fd -s 'path : McCloud')
     library fsadd ~/d/70_Now_Watching/
 
 </details>
 
-### Wake up to your own music (via termux)
+### Music alarm clock (via termux crontab)
+
+Wake up to your own music
 
-    30 9 * * * lb listen ./audio.db
+    30 7 * * * lb listen ./audio.db
 
-### Wake up to your own music _only when you are not home_ (computer on local-only IP)
+Wake up to your own music _only when you are *not* home_ (computer on local-only IP)
 
-    30 9 * * * timeout 0.4 nc -z 192.168.1.12 22 || lb listen --random
+    30 7 * * * timeout 0.4 nc -z 192.168.1.12 22 || lb listen --random
 
-### Wake up to your own music on your Chromecast speaker group _only when you are home_
+Wake up to your own music on your Chromecast speaker group _only when you are home_
 
-    30 9 * * * ssh 192.168.1.12 lb listen --random --play-in-order --cast --cast-to "Bedroom pair"
+    30 7 * * * ssh 192.168.1.12 lb listen --cast --cast-to "Bedroom pair"
 
 ### Pipe to [lowcharts](https://github.com/juan-leon/lowcharts)
 
 <details><summary>$ lb watch -p f -col time_created | lowcharts timehist -w 80</summary>
 
     Matches: 445183.
     Each ∎ represents a count of 1896
@@ -768,17 +798,18 @@
 
 ![fps](https://user-images.githubusercontent.com/7908073/184738438-ee566a4b-2da0-4e6d-a4b3-9bfca036aa2a.png)
 
 </details>
 
 ### Pipe to rsync
 
-<details><summary>Copy or move files to your phone via syncthing</summary>
+<details><summary>Move files to your phone via syncthing</summary>
 
-I use rsync to move files instead of copy-on-write duplication because I want deletions to stick.
+I used to use rsync to move files because I want deletions to stick.
+I now use `lb relmv`. But this is still a good rsync example:
 
     function mrmusic
         rsync -a --remove-source-files --files-from=(
             library lt ~/lb/audio.db -s /mnt/d/80_Now_Listening/ -p f \
             --moved /mnt/d/80_Now_Listening/ /mnt/d/ | psub
         ) /mnt/d/80_Now_Listening/ /mnt/d/
```


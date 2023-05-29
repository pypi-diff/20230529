# Comparing `tmp/xklb-1.29.1.tar.gz` & `tmp/xklb-1.29.2.tar.gz`

## Comparing `xklb-1.29.1.tar` & `xklb-1.29.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.1/.gitattributes
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 xklb-1.29.1/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.1/Windows.md
--rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.1/pdm.lock
--rw-r--r--   0        0        0    17058 2020-02-02 00:00:00.000000 xklb-1.29.1/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.1/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.1/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/__init__.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/books.py
--rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/consts.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/dl_config.py
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/dl_extract.py
--rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/hn_extract.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/lb.py
--rw-r--r--   0        0        0    38063 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/playback.py
--rw-r--r--   0        0        0    32826 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/praw_extract.py
--rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/search.py
--rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/stats.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/tabs_extract.py
--rw-r--r--   0        0        0    23483 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/tube_backend.py
--rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/tube_extract.py
--rw-r--r--   0        0        0    34064 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.1/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.1/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.1/LICENSE
--rw-r--r--   0        0        0    41442 2020-02-02 00:00:00.000000 xklb-1.29.1/README.md
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 xklb-1.29.1/pyproject.toml
--rw-r--r--   0        0        0    45038 2020-02-02 00:00:00.000000 xklb-1.29.1/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.2/.gitattributes
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 xklb-1.29.2/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.2/Windows.md
+-rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.2/pdm.lock
+-rw-r--r--   0        0        0    17058 2020-02-02 00:00:00.000000 xklb-1.29.2/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.2/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.2/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/__init__.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/books.py
+-rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/consts.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/dl_config.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/dl_extract.py
+-rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/hn_extract.py
+-rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/lb.py
+-rw-r--r--   0        0        0    38064 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/playback.py
+-rw-r--r--   0        0        0    32804 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/praw_extract.py
+-rw-r--r--   0        0        0     8215 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/search.py
+-rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/stats.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/tube_extract.py
+-rw-r--r--   0        0        0    34031 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.2/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.2/LICENSE
+-rw-r--r--   0        0        0    41442 2020-02-02 00:00:00.000000 xklb-1.29.2/README.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.29.2/pyproject.toml
+-rw-r--r--   0        0        0    45038 2020-02-02 00:00:00.000000 xklb-1.29.2/PKG-INFO
```

### Comparing `xklb-1.29.1/TODO` & `xklb-1.29.2/TODO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-search: get title from media table
-
--- update fish functions to use --subs --auto-subs
-
 - wt history
     print player.historical_usage
 
+- search: get title from media table
+
+- wt/lt/search join and use fts on both tables, threading ?
+
 - scan bpm and key sig  https://github.com/aubio/aubio https://github.com/tyiannak/pyAudioAnalysis
 
 - CLI EDA tool
 
 - CLI incremental diff (SQLITE, NDJSON, CSV)
 
     compare 100 rows at a time using primary key
```

### Comparing `xklb-1.29.1/Windows.md` & `xklb-1.29.2/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/pdm.lock` & `xklb-1.29.2/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/readme.py` & `xklb-1.29.2/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.29.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.29.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/.github/workflows/push.yaml` & `xklb-1.29.2/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/sql/transfer.sql` & `xklb-1.29.2/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/av.py` & `xklb-1.29.2/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/books.py` & `xklb-1.29.2/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/consts.py` & `xklb-1.29.2/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/db.py` & `xklb-1.29.2/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/dl_config.py` & `xklb-1.29.2/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/dl_extract.py` & `xklb-1.29.2/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/fs_extract.py` & `xklb-1.29.2/xklb/fs_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,25 +58,31 @@
         help="Create image database",
     )
     parser.set_defaults(profile=DBType.video)
     parser.add_argument("--scan-all-files", "-a", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
 
     parser.add_argument(
-        "--io-multiplier", type=float, default=1.0, help="Especially useful for text, image, filesystem db types"
+        "--io-multiplier",
+        type=float,
+        default=1.0,
+        help="Especially useful for text, image, filesystem db types",
     )
     parser.add_argument("--ocr", "--OCR", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--speech-recognition", "--speech", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--scan-subtitles", "--scan-subtitle", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--extra-media-data", default={})
     parser.add_argument("--extra-playlist-data", default={})
 
     parser.add_argument("--delete-unplayable", action="store_true")
     parser.add_argument(
-        "--check-corrupt", type=float, default=0.0, help="check that 0 to 100 percent of media decodes correctly"
+        "--check-corrupt",
+        type=float,
+        default=0.0,
+        help="check that 0 to 100 percent of media decodes correctly",
     )
     parser.add_argument("--delete-corrupt", type=float, help="delete media that is more corrupt than this threshold")
     parser.add_argument("--force", "-f", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
```

### Comparing `xklb-1.29.1/xklb/gui.py` & `xklb-1.29.2/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/hn_extract.py` & `xklb-1.29.2/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/lb.py` & `xklb-1.29.2/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/play_actions.py` & `xklb-1.29.2/xklb/play_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -798,15 +798,15 @@
             args.partial,
             args.lower,
             args.upper,
             args.safe,
             args.play_in_order >= consts.SIMILAR,
             args.related >= consts.RELATED,
             args.cluster,
-        ]
+        ],
     ):
         player.printer(args, query, bindings)
         return
 
     media = list(args.db.query(query, bindings))
     log.debug("query: %s", t.elapsed())
```

### Comparing `xklb-1.29.1/xklb/playback.py` & `xklb-1.29.2/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/player.py` & `xklb-1.29.2/xklb/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,19 +430,19 @@
             SELECT
                 {args.select_sql}
             FROM {'media' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else args.table}
             WHERE 1=1
                 and path like :candidate
                 {filter_args_sql(args, m_columns)}
                 {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER else (" ".join(args.filter_sql) or '')}
-                {"and path not in ({})".format(",".join([":ignore_path{}".format(i) for i in range(len(ignore_paths))])) if len(ignore_paths) > 0 else ''}
+                {"and path not in ({})".format(",".join([f":ignore_path{i}" for i in range(len(ignore_paths))])) if len(ignore_paths) > 0 else ''}
             ORDER BY play_count, path
             LIMIT 1000
             """
-        ignore_path_params = {"ignore_path{}".format(i): value for i, value in enumerate(ignore_paths)}
+        ignore_path_params = {f"ignore_path{i}": value for i, value in enumerate(ignore_paths)}
         bindings = {"candidate": candidate + "%", **ignore_path_params}
         if args.play_in_order >= consts.SIMILAR_NO_FILTER:
             if args.include or args.exclude:
                 bindings = {**bindings, "query": args.filter_bindings["query"]}
         else:
             bindings = {**bindings, **args.filter_bindings}
 
@@ -466,15 +466,15 @@
 
 def get_related_media(args, m: Dict) -> List[Dict]:
     m_columns = args.db["media"].columns_dict
     m_columns.update(rank=int)
 
     m = args.db["media"].get(m["path"])
     words = set(
-        utils.conform(utils.extract_words(m.get(k)) for k in m.keys() if k in db.config["media"]["search_columns"])
+        utils.conform(utils.extract_words(m.get(k)) for k in m if k in db.config["media"]["search_columns"]),
     )
     args.include = sorted(words, key=len, reverse=True)[:100]
     args.table = db.fts_flexible_search(args)
 
     query = f"""
         SELECT
             {args.select_sql}, rank
@@ -494,15 +494,15 @@
         bindings = {**bindings, "query": args.filter_bindings["query"]}
     else:
         bindings = {**bindings, **args.filter_bindings}
 
     related_videos = list(args.db.query(query, bindings))
     log.debug(related_videos)
 
-    return [m] + related_videos
+    return [m, *related_videos]
 
 
 def watch_chromecast(args, m: dict, subtitles_file=None) -> Optional[subprocess.CompletedProcess]:
     if "vlc" in args.player:
         catt_log = cmd(
             "vlc",
             "--sout",
```

### Comparing `xklb-1.29.1/xklb/praw_extract.py` & `xklb-1.29.2/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/search.py` & `xklb-1.29.2/xklb/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     Search and open file
     $ library search fts.db dashi --open
 """,
     )
     parser.add_argument("--open", "--play", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
-    parser.add_argument("--overlap", type=int, default=7, help=argparse.SUPPRESS)
+    parser.add_argument("--overlap", type=int, default=8, help=argparse.SUPPRESS)
     parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--sort", "-u", nargs="+", default=["path", "time"], help=argparse.SUPPRESS)
     parser.add_argument("--csv", action="store_true")
     parser.add_argument("--json", action="store_true")
     parser.add_argument("--table", action="store_true")
@@ -157,27 +157,35 @@
 
 
 def merge_captions(args, captions):
     def get_end(caption):
         return caption["time"] + (len(caption["text"]) / 4.2 / 220 * 60)
 
     merged_captions = []
-    for path, group in groupby(captions, key=lambda x: x["path"]):
+    for path, group in groupby(
+        captions, key=lambda x: x["path"]
+    ):  # group by only does contiguous items with the same key
         group = list(group)
         merged_group = {"path": path, "time": group[0]["time"], "end": get_end(group[0]), "text": group[0]["text"]}
         for i in range(1, len(group)):
-            if abs(group[i]["time"] - merged_group["end"]) <= args.overlap:
-                merged_group["end"] = get_end(group[i])
-                merged_group["text"] += ". " + group[i]["text"]
+            end = get_end(group[i])
+
+            if (
+                abs(group[i]["time"] - merged_group["end"]) <= args.overlap
+                or abs(group[i]["time"] - merged_group["time"]) <= args.overlap
+            ):
+                merged_group["end"] = end
+                if group[i]["text"] not in merged_group["text"]:
+                    merged_group["text"] += ". " + group[i]["text"]
             else:
                 merged_captions.append(merged_group)
                 merged_group = {
                     "path": path,
                     "time": group[i]["time"],
-                    "end": get_end(group[i]),
+                    "end": end,
                     "text": group[i]["text"],
                 }
         merged_captions.append(merged_group)
 
     return merged_captions
```

### Comparing `xklb-1.29.1/xklb/stats.py` & `xklb-1.29.2/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/subtitle.py` & `xklb-1.29.2/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/tabs_actions.py` & `xklb-1.29.2/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/tabs_extract.py` & `xklb-1.29.2/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/tube_backend.py` & `xklb-1.29.2/xklb/tube_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
                 "subtitleslangs": args.subtitle_languages,
                 "extract_flat": False,
                 "lazy_playlist": False,
                 "check_formats": False,
                 "skip_download": True,
                 "outtmpl": {
                     "default": str(
-                        Path(f"{consts.SUB_TEMP_DIR}/%(uploader,uploader_id)s/%(title).200B_[%(id).60B].%(ext)s")
+                        Path(f"{consts.SUB_TEMP_DIR}/%(uploader,uploader_id)s/%(title).200B_[%(id).60B].%(ext)s"),
                     ),
                 },
                 "ignoreerrors": True,
             },
             playlist_opts=playlist_dl_opts,
         ),
     ) as ydl:
```

### Comparing `xklb-1.29.1/xklb/tube_extract.py` & `xklb-1.29.2/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/utils.py` & `xklb-1.29.2/xklb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
         .replace("[", " ")
         .replace("(", " ")
         .replace("]", " ")
         .replace(")", " ")
         .replace("{", " ")
         .replace("}", " ")
         .replace("_", " ")
-        .replace("-", " ")
+        .replace("-", " "),
     )
 
 
 def safe_int(s) -> Optional[int]:
     try:
         return int(float(s))
     except Exception:
@@ -1030,23 +1030,23 @@
         scans.append(math.floor(media_duration - scan_duration))
 
     return scans, scan_duration
 
 
 def decode_full_scan(path):
     output = ffmpeg.input(path).output("/dev/null", f="null")
-    error_log = ffmpeg.run(output, quiet=True)
+    ffmpeg.run(output, quiet=True)
 
 
 def decode_quick_scan(path, scans, scan_duration=3):
     fail_count = 0
     for scan in scans:
         try:
             output = ffmpeg.input(path, ss=scan).output("/dev/null", t=scan_duration, f="null")
-            error_log = ffmpeg.run(output, quiet=True)
+            ffmpeg.run(output, quiet=True)
         except ffmpeg.Error:
             fail_count += 1
 
     return (fail_count / len(scans)) * 100
 
 
 def fast_glob(path_dir, limit=100):
@@ -1063,15 +1063,15 @@
 def load_spacy_model(model=None):
     try:
         import spacy
     except ModuleNotFoundError:
         log.error("Install spaCy and sklearn to use:")
         log.error("pip install spacy sklearn")
         log.error("python -m spacy download en_core_web_sm")
-        exit(1)
+        sys.exit(1)
 
     if model:
         return spacy.load(model)
 
     model_sizes = ["lg", "md", "sm"]
     loaded_model = None
 
@@ -1083,15 +1083,15 @@
             pass
 
     if loaded_model:
         return loaded_model
 
     log.error("Language model not found. Download a model first using the following commands:")
     log.error("python -m spacy download en_core_web_sm")
-    exit(1)
+    sys.exit(1)
 
 
 def cluster_paths(paths, model=None, n_clusters=None):
     nlp = load_spacy_model(model)
 
     from sklearn.cluster import KMeans
     from sklearn.feature_extraction.text import TfidfVectorizer
@@ -1134,15 +1134,15 @@
         if not (char in ":,_-;. " or char.isdigit()):
             return False
     return True
 
 
 def is_generic_title(title):
     return (
-        (len(title) <= 12 and (title.startswith("Chapter") or title.startswith("Scene")))
+        (len(title) <= 12 and (title.startswith(("Chapter", "Scene"))))
         or "Untitled Chapter" in title
         or is_timecode_like(title)
         or title.isdigit()
     )
 
 
 def write_csv_to_stdout(data):
```

### Comparing `xklb-1.29.1/xklb/scripts/bigdirs.py` & `xklb-1.29.2/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/christen.py` & `xklb-1.29.2/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/cluster_sort.py` & `xklb-1.29.2/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/copy_play_counts.py` & `xklb-1.29.2/xklb/scripts/copy_play_counts.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,24 +39,24 @@
         """
         SELECT
             *
         FROM
             src.media
         WHERE
             src.media.play_count > 0
-        """
+        """,
     )
 
     modified_row_count = 0
     with args.db.conn:
         for d in copy_counts:
             renamed_path = d["path"].replace(args.source_prefix, args.target_prefix, 1)
             log.debug(renamed_path)
 
-            sql = f"""
+            sql = """
             UPDATE
                 main.media
             SET
                 play_count = :play_count
                 , time_played = :time_played
                 , playhead = :playhead
             WHERE
```

### Comparing `xklb-1.29.1/xklb/scripts/dedupe.py` & `xklb-1.29.2/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/merge_dbs.py` & `xklb-1.29.2/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/merge_online_local.py` & `xklb-1.29.2/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/move_list.py` & `xklb-1.29.2/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/optimize_db.py` & `xklb-1.29.2/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/redownload.py` & `xklb-1.29.2/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/relmv.py` & `xklb-1.29.2/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/scatter.py` & `xklb-1.29.2/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/streaming_tab_loader.py` & `xklb-1.29.2/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/mining/data.py` & `xklb-1.29.2/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/mining/extract_links.py` & `xklb-1.29.2/xklb/scripts/mining/extract_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         from selenium import webdriver
 
         if which("firefox"):
             driver = webdriver.Firefox()
         else:
             driver = webdriver.Chrome()
 
-    with open(args.filename, "r") as f:
+    with open(args.filename) as f:
         for line in f:
             url = line.rstrip("\n")
             if url in ["", '""', "\n"]:
                 continue
 
             if args.scroll:
                 markup = get_page_infinite_scroll(driver, url)
```

### Comparing `xklb-1.29.1/xklb/scripts/mining/nouns.py` & `xklb-1.29.2/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/mining/pushshift.py` & `xklb-1.29.2/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.29.2/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/xklb/assets/kotobago.png` & `xklb-1.29.2/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/.gitignore` & `xklb-1.29.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/LICENSE` & `xklb-1.29.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.29.1/README.md` & `xklb-1.29.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     library tabs tabs.db -L 1  # open one tab
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.29.001)
+    xk media library subcommands (v1.29.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.29.1/pyproject.toml` & `xklb-1.29.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 ignore = [
   "ANN001",
   "ANN002",
   "ANN003",
   "ANN101",
   "ANN204",
   "BLE001",
+  "C401",
   "C901",
   "D100",
   "D101",
   "D102",
   "D103",
   "D104",
   "D107",
@@ -123,14 +124,16 @@
   "S311",
   "S324",
   "S603",
   "S606",
   "SIM103",
   "SIM105",
   "SIM108",
+  "SIM110",
+  "SIM111",
   "SIM114",
   "T100",
   "T201",
   "TRY003",
   "TRY300",
   "TRY301",
 ]
```

### Comparing `xklb-1.29.1/PKG-INFO` & `xklb-1.29.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.29.1
+Version: 1.29.2
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -219,15 +219,15 @@
     library tabs tabs.db -L 1  # open one tab
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.29.001)
+    xk media library subcommands (v1.29.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```


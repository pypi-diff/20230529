# Comparing `tmp/xklb-1.29.3.tar.gz` & `tmp/xklb-1.29.4.tar.gz`

## Comparing `xklb-1.29.3.tar` & `xklb-1.29.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.3/.gitattributes
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 xklb-1.29.3/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.3/Windows.md
--rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.3/pdm.lock
--rw-r--r--   0        0        0    19035 2020-02-02 00:00:00.000000 xklb-1.29.3/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.3/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.3/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/__init__.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/books.py
--rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/consts.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/dl_config.py
--rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/dl_extract.py
--rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/gui.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/hn_extract.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/lb.py
--rw-r--r--   0        0        0    24360 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/playback.py
--rw-r--r--   0        0        0    32804 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/player.py
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/praw_extract.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/search.py
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/stats.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/subtitle.py
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/tabs_extract.py
--rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/tube_backend.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/tube_extract.py
--rw-r--r--   0        0        0    54097 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/usage.py
--rw-r--r--   0        0        0    34031 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.3/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.3/LICENSE
--rw-r--r--   0        0        0    76267 2020-02-02 00:00:00.000000 xklb-1.29.3/README.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.29.3/pyproject.toml
--rw-r--r--   0        0        0    79863 2020-02-02 00:00:00.000000 xklb-1.29.3/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.4/.gitattributes
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 xklb-1.29.4/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.4/Windows.md
+-rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.4/pdm.lock
+-rw-r--r--   0        0        0    19035 2020-02-02 00:00:00.000000 xklb-1.29.4/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.4/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.4/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/__init__.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/books.py
+-rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/consts.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/dl_config.py
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/gui.py
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/hn_extract.py
+-rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/lb.py
+-rw-r--r--   0        0        0    24360 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/playback.py
+-rw-r--r--   0        0        0    32804 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/player.py
+-rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/search.py
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/stats.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/subtitle.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/tube_extract.py
+-rw-r--r--   0        0        0    54097 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/usage.py
+-rw-r--r--   0        0        0    34316 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.4/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.4/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.4/LICENSE
+-rw-r--r--   0        0        0    76267 2020-02-02 00:00:00.000000 xklb-1.29.4/README.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.29.4/pyproject.toml
+-rw-r--r--   0        0        0    79863 2020-02-02 00:00:00.000000 xklb-1.29.4/PKG-INFO
```

### Comparing `xklb-1.29.3/TODO` & `xklb-1.29.4/TODO`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-- merge dbs --only-new-rows --only-target-columns
-
 - wt history
     print player.historical_usage
 
 - sqlite-utils transform chickens.db chickens --pk id
 
 use rowid alias instead of string pks
```

### Comparing `xklb-1.29.3/Windows.md` & `xklb-1.29.4/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/pdm.lock` & `xklb-1.29.4/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/readme.py` & `xklb-1.29.4/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.29.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.29.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/.github/workflows/push.yaml` & `xklb-1.29.4/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/sql/transfer.sql` & `xklb-1.29.4/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/av.py` & `xklb-1.29.4/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/books.py` & `xklb-1.29.4/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/consts.py` & `xklb-1.29.4/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/db.py` & `xklb-1.29.4/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/dl_config.py` & `xklb-1.29.4/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/dl_extract.py` & `xklb-1.29.4/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/fs_extract.py` & `xklb-1.29.4/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/gui.py` & `xklb-1.29.4/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/hn_extract.py` & `xklb-1.29.4/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/lb.py` & `xklb-1.29.4/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/play_actions.py` & `xklb-1.29.4/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/playback.py` & `xklb-1.29.4/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/player.py` & `xklb-1.29.4/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/praw_extract.py` & `xklb-1.29.4/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/search.py` & `xklb-1.29.4/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/stats.py` & `xklb-1.29.4/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/subtitle.py` & `xklb-1.29.4/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/tabs_actions.py` & `xklb-1.29.4/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/tabs_extract.py` & `xklb-1.29.4/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/tube_backend.py` & `xklb-1.29.4/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/tube_extract.py` & `xklb-1.29.4/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/usage.py` & `xklb-1.29.4/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/utils.py` & `xklb-1.29.4/xklb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -712,14 +712,24 @@
 def col_hhmmss(tbl: List[Dict], col: str) -> List[Dict]:
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
             tbl[idx][col] = seconds_to_hhmmss(tbl[idx][col])
     return tbl
 
 
+class ArgparseList(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        items = getattr(namespace, self.dest, [])
+
+        for value in values or []:
+            items.extend(value.split(","))
+
+        setattr(namespace, self.dest, items)
+
+
 class ArgparseDict(argparse.Action):
     def __call__(self, parser, args, values, option_string=None):
         try:
             d = {}
             k_eq_v = list(flatten([val.split(" ") for val in values]))
             for s in k_eq_v:
                 k, v = s.split("=")
```

### Comparing `xklb-1.29.3/xklb/scripts/bigdirs.py` & `xklb-1.29.4/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/christen.py` & `xklb-1.29.4/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/cluster_sort.py` & `xklb-1.29.4/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/copy_play_counts.py` & `xklb-1.29.4/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/dedupe.py` & `xklb-1.29.4/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/merge_dbs.py` & `xklb-1.29.4/xklb/scripts/merge_dbs.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 from xklb import db, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library merge-dbs", usage=usage.merge_dbs)
-    parser.add_argument("database")
-    parser.add_argument("source_dbs", nargs="+")
-    parser.add_argument("--pk")
-    parser.add_argument("--table", "-t", help="Limit to specific table(s)")
+    parser.add_argument("--pk", nargs="+", action=utils.ArgparseList, help="Comma separated primary keys")
+    parser.add_argument("--table", "-t", nargs="+", action=utils.ArgparseList, help="Limit to specific table(s)")
     parser.add_argument("--upsert", action="store_true")
+    parser.add_argument("--ignore", "--only-new-rows", action="store_true")
+    parser.add_argument("--only-target-columns", action="store_true")
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
+
+    parser.add_argument("database")
+    parser.add_argument("source_dbs", nargs="+")
     args = parser.parse_intermixed_args()
 
     if args.db:
         args.database = args.db
     Path(args.database).touch()
     args.db = db.connect(args)
 
-    if args.table:
-        args.table = args.table.split(",")
-
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
 
 def merge_db(args, source_db) -> None:
     source_db = str(Path(source_db).resolve())
@@ -37,28 +37,37 @@
         if args.table and table not in args.table:
             log.info("[%s]: Skipping %s", source_db, table)
             continue
         else:
             log.info("[%s]: %s", source_db, table)
 
         source_columns = s_db[table].columns_dict
+        if args.only_target_columns:
+            target_columns = args.db[table].columns_dict
+            source_columns = [s for s in source_columns if s in target_columns]
+
         log.info("[%s]: %s", table, source_columns)
-        primary_keys = [s for s in args.pk.split(",") if s in source_columns]
+        source_table_pks = [s for s in args.pk if s in source_columns]
 
         kwargs = {}
-        if primary_keys:
-            log.info("[%s]: Using %s as primary key(s)", table, ",".join(primary_keys))
-            kwargs["pk"] = primary_keys
+        if source_table_pks:
+            log.info("[%s]: Using %s as primary key(s)", table, ", ".join(source_table_pks))
+            kwargs["pk"] = source_table_pks
 
         data = s_db[table].rows
+        data = ({k: v for k, v in d.items() if k in source_columns} for d in data)
         with args.db.conn:
-            if args.upsert:
-                args.db[table].upsert_all(data, alter=True, **kwargs)
-            else:
-                args.db[table].insert_all(data, alter=True, replace=True, **kwargs)
+            args.db[table].insert_all(
+                data,
+                alter=True,
+                ignore=args.ignore,
+                replace=not args.ignore,
+                upsert=args.upsert,
+                **kwargs,
+            )
 
 
 def merge_dbs() -> None:
     args = parse_args()
     for s_db in args.source_dbs:
         merge_db(args, s_db)
```

### Comparing `xklb-1.29.3/xklb/scripts/merge_online_local.py` & `xklb-1.29.4/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/move_list.py` & `xklb-1.29.4/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/optimize_db.py` & `xklb-1.29.4/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/redownload.py` & `xklb-1.29.4/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/relmv.py` & `xklb-1.29.4/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/scatter.py` & `xklb-1.29.4/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/streaming_tab_loader.py` & `xklb-1.29.4/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/mining/data.py` & `xklb-1.29.4/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/mining/extract_links.py` & `xklb-1.29.4/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/mining/nouns.py` & `xklb-1.29.4/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/mining/pushshift.py` & `xklb-1.29.4/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.29.4/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/xklb/assets/kotobago.png` & `xklb-1.29.4/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/.gitignore` & `xklb-1.29.4/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/LICENSE` & `xklb-1.29.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/README.md` & `xklb-1.29.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.29.003)
+    xk media library subcommands (v1.29.004)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.29.3/pyproject.toml` & `xklb-1.29.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.29.3/PKG-INFO` & `xklb-1.29.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.29.3
+Version: 1.29.4
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -223,15 +223,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.29.003)
+    xk media library subcommands (v1.29.004)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```


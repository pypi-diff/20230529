# Comparing `tmp/xklb-1.29.2.tar.gz` & `tmp/xklb-1.29.3.tar.gz`

## Comparing `xklb-1.29.2.tar` & `xklb-1.29.3.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.2/.gitattributes
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 xklb-1.29.2/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.2/Windows.md
--rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.2/pdm.lock
--rw-r--r--   0        0        0    17058 2020-02-02 00:00:00.000000 xklb-1.29.2/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.2/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.2/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/__init__.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/books.py
--rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/consts.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/dl_config.py
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/dl_extract.py
--rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/hn_extract.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/lb.py
--rw-r--r--   0        0        0    38064 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/playback.py
--rw-r--r--   0        0        0    32804 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/praw_extract.py
--rw-r--r--   0        0        0     8215 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/search.py
--rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/stats.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/tabs_extract.py
--rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/tube_backend.py
--rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/tube_extract.py
--rw-r--r--   0        0        0    34031 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.2/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.2/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.2/LICENSE
--rw-r--r--   0        0        0    41442 2020-02-02 00:00:00.000000 xklb-1.29.2/README.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.29.2/pyproject.toml
--rw-r--r--   0        0        0    45038 2020-02-02 00:00:00.000000 xklb-1.29.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.3/.gitattributes
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 xklb-1.29.3/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.3/Windows.md
+-rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.3/pdm.lock
+-rw-r--r--   0        0        0    19035 2020-02-02 00:00:00.000000 xklb-1.29.3/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.3/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.3/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/__init__.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/books.py
+-rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/consts.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/dl_config.py
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/gui.py
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/hn_extract.py
+-rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/lb.py
+-rw-r--r--   0        0        0    24360 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/playback.py
+-rw-r--r--   0        0        0    32804 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/player.py
+-rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/search.py
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/stats.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/subtitle.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/tube_extract.py
+-rw-r--r--   0        0        0    54097 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/usage.py
+-rw-r--r--   0        0        0    34031 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.3/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.3/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.3/LICENSE
+-rw-r--r--   0        0        0    76267 2020-02-02 00:00:00.000000 xklb-1.29.3/README.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.29.3/pyproject.toml
+-rw-r--r--   0        0        0    79863 2020-02-02 00:00:00.000000 xklb-1.29.3/PKG-INFO
```

### Comparing `xklb-1.29.2/TODO` & `xklb-1.29.3/TODO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,21 @@
+- merge dbs --only-new-rows --only-target-columns
+
 - wt history
     print player.historical_usage
 
+- sqlite-utils transform chickens.db chickens --pk id
+
+use rowid alias instead of string pks
+
+[author_id] INTEGER REFERENCES [authors]([id])
+db["dogs"].add_column("species_id", fk="species", fk_col="ref")
+
+table.transform(pk=None)
+
 - search: get title from media table
 
 - wt/lt/search join and use fts on both tables, threading ?
 
 - scan bpm and key sig  https://github.com/aubio/aubio https://github.com/tyiannak/pyAudioAnalysis
 
 - CLI EDA tool
```

### Comparing `xklb-1.29.2/Windows.md` & `xklb-1.29.3/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/pdm.lock` & `xklb-1.29.3/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -569,15 +569,15 @@
 name = "packaging"
 version = "23.1"
 requires_python = ">=3.7"
 summary = "Core utilities for Python packages"
 
 [[package]]
 name = "pandas"
-version = "2.0.1"
+version = "2.0.2"
 requires_python = ">=3.8"
 summary = "Powerful data structures for data analysis, time series, and statistics"
 dependencies = [
     "numpy>=1.20.3; python_version < \"3.10\"",
     "numpy>=1.21.0; python_version >= \"3.10\"",
     "numpy>=1.23.2; python_version >= \"3.11\"",
     "python-dateutil>=2.8.2",
@@ -2396,40 +2396,40 @@
     {url = "https://files.pythonhosted.org/packages/f4/18/a84b513905e1ed78529084967ca0b937f6ec45df200f908c4393aefddd79/orjson-3.8.14-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:f4ac01a3db4e6a98a8ad1bb1a3e8bfc777928939e87c04e93e0d5006df574a4b"},
     {url = "https://files.pythonhosted.org/packages/f9/fa/35ba54c9ff8ba0c0759d8a496095f9fdf0ff7c18182c330784f6b3025754/orjson-3.8.14-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9393a63cb0424515ec5e434078b3198de6ec9e057f1d33bad268683935f0a5d5"},
 ]
 "packaging 23.1" = [
     {url = "https://files.pythonhosted.org/packages/ab/c3/57f0601a2d4fe15de7a553c00adbc901425661bf048f2a22dfc500caf121/packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {url = "https://files.pythonhosted.org/packages/b9/6c/7c6658d258d7971c5eb0d9b69fa9265879ec9a9158031206d47800ae2213/packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
-"pandas 2.0.1" = [
-    {url = "https://files.pythonhosted.org/packages/16/75/924e3a52c35cb105a152d29622d0f06bb0f48a677e77ddd6e11ef0004164/pandas-2.0.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e09a53a4fe8d6ae2149959a2d02e1ef2f4d2ceb285ac48f74b79798507e468b4"},
-    {url = "https://files.pythonhosted.org/packages/17/10/712e0566d1f561d1fcbb8f620523bc1777c7f1183365b5747b74e0585637/pandas-2.0.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:70a996a1d2432dadedbb638fe7d921c88b0cc4dd90374eab51bb33dc6c0c2a12"},
-    {url = "https://files.pythonhosted.org/packages/32/49/d7240d653397a74f181015bbf0a412098e54aa72f59660d0dd82e336fac8/pandas-2.0.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:af2449e9e984dfad39276b885271ba31c5e0204ffd9f21f287a245980b0e4091"},
-    {url = "https://files.pythonhosted.org/packages/41/07/4bf208b31ae6e78a70baa706c5cb90c02d458d418a707c193466bf8cd4e5/pandas-2.0.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:909a72b52175590debbf1d0c9e3e6bce2f1833c80c76d80bd1aa09188be768e5"},
-    {url = "https://files.pythonhosted.org/packages/41/77/a8210fab9a40a3546ab24f69e81c77539818d4379b6255a4510892d91015/pandas-2.0.1-cp38-cp38-win_amd64.whl", hash = "sha256:03e677c6bc9cfb7f93a8b617d44f6091613a5671ef2944818469be7b42114a00"},
-    {url = "https://files.pythonhosted.org/packages/4b/1a/252a5933e9c7fcf632b34d5a269d04b313b0181a58eb1395377503eccc7c/pandas-2.0.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3d099ecaa5b9e977b55cd43cf842ec13b14afa1cfa51b7e1179d90b38c53ce6a"},
-    {url = "https://files.pythonhosted.org/packages/55/4f/934c0be7d9d50f9c0ca306281e3fc306b17b086c672deed55c6fe55ab2c6/pandas-2.0.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:a37ee35a3eb6ce523b2c064af6286c45ea1c7ff882d46e10d0945dbda7572753"},
-    {url = "https://files.pythonhosted.org/packages/6c/e0/73987b6ecc7246e02ab557240843f93fd5adf45d1355abb458aa1f2a0932/pandas-2.0.1.tar.gz", hash = "sha256:19b8e5270da32b41ebf12f0e7165efa7024492e9513fb46fb631c5022ae5709d"},
-    {url = "https://files.pythonhosted.org/packages/6f/cf/d52394af3194f41db6cf99ec0975e913ad1bab14b69962d7ae7da5e4f01a/pandas-2.0.1-cp310-cp310-win32.whl", hash = "sha256:12bd6618e3cc737c5200ecabbbb5eaba8ab645a4b0db508ceeb4004bb10b060e"},
-    {url = "https://files.pythonhosted.org/packages/90/30/8b857447b0f4b59d5bd84e934e82ef8c82b73d71d1c9611c8aaaa8d44a50/pandas-2.0.1-cp310-cp310-win_amd64.whl", hash = "sha256:2b6fe5f7ce1cba0e74188c8473c9091ead9b293ef0a6794939f8cc7947057abd"},
-    {url = "https://files.pythonhosted.org/packages/91/ff/6af7586c9e8982dcf7078adfba1b0af244ae4dd7e5cbd617c24be9210ed5/pandas-2.0.1-cp39-cp39-win_amd64.whl", hash = "sha256:99f7192d8b0e6daf8e0d0fd93baa40056684e4b4aaaef9ea78dff34168e1f2f0"},
-    {url = "https://files.pythonhosted.org/packages/93/1f/85327a36a8fdc441a58424cfeb9104c2fa884eea1c9249a3c061c5c805a7/pandas-2.0.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:6c0853d487b6c868bf107a4b270a823746175b1932093b537b9b76c639fc6f7e"},
-    {url = "https://files.pythonhosted.org/packages/95/df/ed5395174b7659e13444690073faaf3fcd5b7574e2a5180a2c44796c6728/pandas-2.0.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:7bbf173d364130334e0159a9a034f573e8b44a05320995127cf676b85fd8ce86"},
-    {url = "https://files.pythonhosted.org/packages/a3/40/eca46f6af07a83ea3b8706586b2d8a28c01bdccee789d24f2ccc5e148b28/pandas-2.0.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0a514ae436b23a92366fbad8365807fc0eed15ca219690b3445dcfa33597a5cc"},
-    {url = "https://files.pythonhosted.org/packages/a3/6b/adebe4415a929833cce8f63465b19386382ec855ab161a21ab08344a7a43/pandas-2.0.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fe7914d8ddb2d54b900cec264c090b88d141a1eed605c9539a187dbc2547f022"},
-    {url = "https://files.pythonhosted.org/packages/ac/99/ebdcc8665b7a94bf4dba22cbd6883ee633caa760b149ffe63cc1957b90ae/pandas-2.0.1-cp38-cp38-win32.whl", hash = "sha256:a2564629b3a47b6aa303e024e3d84e850d36746f7e804347f64229f8c87416ea"},
-    {url = "https://files.pythonhosted.org/packages/b2/4c/e04a85386949b0849c310e980f0e16d970b932f15d8eacd81987b97fe6da/pandas-2.0.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f25e23a03f7ad7211ffa30cb181c3e5f6d96a8e4cb22898af462a7333f8a74eb"},
-    {url = "https://files.pythonhosted.org/packages/b3/3b/acb903edc6d4a9272af71181eee2840b0b1ca104ea3545127393246b7c32/pandas-2.0.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:00959a04a1d7bbc63d75a768540fb20ecc9e65fd80744c930e23768345a362a7"},
-    {url = "https://files.pythonhosted.org/packages/c9/35/5337271d6cd24ec58d44991abe8adc6686e6796fc5ac893bcefa905b7423/pandas-2.0.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:320b180d125c3842c5da5889183b9a43da4ebba375ab2ef938f57bf267a3c684"},
-    {url = "https://files.pythonhosted.org/packages/d2/cb/7cb0c973d7ae336f46a6e2b29c84496fadde49fe651739efdc2035af1779/pandas-2.0.1-cp39-cp39-win32.whl", hash = "sha256:90d1d365d77d287063c5e339f49b27bd99ef06d10a8843cf00b1a49326d492c1"},
-    {url = "https://files.pythonhosted.org/packages/e9/d7/ee1b27176addc1236f4a59a9ca105bbdf60424a597ab9b4e13f09e0a816f/pandas-2.0.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:18d22cb9043b6c6804529810f492ab09d638ddf625c5dea8529239607295cb59"},
-    {url = "https://files.pythonhosted.org/packages/f3/32/2fae5c7e886d543c09328301baf1c79cf5e0a111b22dbf01779d97a702f7/pandas-2.0.1-cp311-cp311-win32.whl", hash = "sha256:7b8395d335b08bc8b050590da264f94a439b4770ff16bb51798527f1dd840388"},
-    {url = "https://files.pythonhosted.org/packages/f3/ac/8bfddafc42a0c801902efa2c3f4ee286369df1a4acafc0409a13c458c8bf/pandas-2.0.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6fa0067f2419f933101bdc6001bcea1d50812afbd367b30943417d67fbb99678"},
-    {url = "https://files.pythonhosted.org/packages/f7/56/38f5d7ccd495451979d38dc7d534035989f2dadf183600c53ae5501dff3d/pandas-2.0.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:910df06feaf9935d05247db6de452f6d59820e432c18a2919a92ffcd98f8f79b"},
-    {url = "https://files.pythonhosted.org/packages/fc/79/a3ae8a668af15210d03e06bd8051892cab0826e7be7993d3b1e4a03ab420/pandas-2.0.1-cp311-cp311-win_amd64.whl", hash = "sha256:8db5a644d184a38e6ed40feeb12d410d7fcc36648443defe4707022da127fc35"},
+"pandas 2.0.2" = [
+    {url = "https://files.pythonhosted.org/packages/07/66/a1c77bc7af5358f4404e47a28a0f16d624fffa20ed35ba189d03872023b8/pandas-2.0.2-cp38-cp38-win32.whl", hash = "sha256:6d6d10c2142d11d40d6e6c0a190b1f89f525bcf85564707e31b0a39e3b398e08"},
+    {url = "https://files.pythonhosted.org/packages/0c/71/bc53a6966c6abc4ed7f0a65a897c5bf2569dc727ab349be0d8a245014f44/pandas-2.0.2-cp310-cp310-win_amd64.whl", hash = "sha256:66d00300f188fa5de73f92d5725ced162488f6dc6ad4cecfe4144ca29debe3b8"},
+    {url = "https://files.pythonhosted.org/packages/10/df/3a4b53426bb62b46c4744712f8f7443ec788bd04d167599d55c0244e1c10/pandas-2.0.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c7319b6e68de14e6209460f72a8d1ef13c09fb3d3ef6c37c1e65b35d50b5c145"},
+    {url = "https://files.pythonhosted.org/packages/11/4c/a9be545c613e08b025f12a806b690deb8d0204c83c4a075ca3e88452a768/pandas-2.0.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:30a89d0fec4263ccbf96f68592fd668939481854d2ff9da709d32a047689393b"},
+    {url = "https://files.pythonhosted.org/packages/24/03/e76679b6aba0f3984cf827b763dcc95685af71b0ff7a76777b02f9f48623/pandas-2.0.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:69167693cb8f9b3fc060956a5d0a0a8dbfed5f980d9fd2c306fb5b9c855c814c"},
+    {url = "https://files.pythonhosted.org/packages/2a/49/be958fefa589186b54daaa9a72fa1a2e19e42a2dcab87ee15c8273259da0/pandas-2.0.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:02755de164da6827764ceb3bbc5f64b35cb12394b1024fdf88704d0fa06e0e2f"},
+    {url = "https://files.pythonhosted.org/packages/3c/25/4292916c1f4b7bb4af615e1437b6ec75ba73f0a3463157a7485bc196881a/pandas-2.0.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dd46bde7309088481b1cf9c58e3f0e204b9ff9e3244f441accd220dd3365ce7c"},
+    {url = "https://files.pythonhosted.org/packages/3f/9c/81783576b66ed29c65962d1ec0936e7912c0b6b7917e8f7722a79a363430/pandas-2.0.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:b42b120458636a981077cfcfa8568c031b3e8709701315e2bfa866324a83efa8"},
+    {url = "https://files.pythonhosted.org/packages/54/d7/9e8ff0685d3454a13949e0503bdc789b4bc5bb35989c3948101e71b362cd/pandas-2.0.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:1eb09a242184092f424b2edd06eb2b99d06dc07eeddff9929e8667d4ed44e181"},
+    {url = "https://files.pythonhosted.org/packages/56/60/59fdaf1d0ac5c3314f755562238a38f6f2ee64dfffb3182ee1e29abc7466/pandas-2.0.2-cp39-cp39-win_amd64.whl", hash = "sha256:77550c8909ebc23e56a89f91b40ad01b50c42cfbfab49b3393694a50549295ea"},
+    {url = "https://files.pythonhosted.org/packages/78/ca/fac24e2ff729cfa88c391645842d6010caf88f0c399001e4f8e86ca33d7c/pandas-2.0.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:f908a77cbeef9bbd646bd4b81214cbef9ac3dda4181d5092a4aa9797d1bc7774"},
+    {url = "https://files.pythonhosted.org/packages/9b/52/18c98eb7cc3965faf26b7a49453c2d0145b50143b2e417ead4e97707e2c2/pandas-2.0.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7376e13d28eb16752c398ca1d36ccfe52bf7e887067af9a0474de6331dd948d2"},
+    {url = "https://files.pythonhosted.org/packages/9f/cc/cc8135de2a574fd87940b1d41c9c52d226d3ebc9fc8f6e9f18a7b0a81b57/pandas-2.0.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cf3f0c361a4270185baa89ec7ab92ecaa355fe783791457077473f974f654df5"},
+    {url = "https://files.pythonhosted.org/packages/a4/cb/b0201b3bf6c42a71dd24aef4a686edf775ded116caf811c94d34cb90cc96/pandas-2.0.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:9ebb9f1c22ddb828e7fd017ea265a59d80461d5a79154b49a4207bd17514d122"},
+    {url = "https://files.pythonhosted.org/packages/a6/03/a412957f3c5db6705f9353210120e4a174f5cdd366362e04a6087798b0d9/pandas-2.0.2-cp310-cp310-win32.whl", hash = "sha256:51a93d422fbb1bd04b67639ba4b5368dffc26923f3ea32a275d2cc450f1d1c86"},
+    {url = "https://files.pythonhosted.org/packages/b1/12/618452820245081263c69e055a7fbdea43e141476abc5411bb3c8c830bca/pandas-2.0.2-cp311-cp311-win32.whl", hash = "sha256:7b21cb72958fc49ad757685db1919021d99650d7aaba676576c9e88d3889d456"},
+    {url = "https://files.pythonhosted.org/packages/b4/1d/00603e672fa49f5c75e75c563a3bff98d5f48bb6e7c946e7ec035ecf7795/pandas-2.0.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:0a1e0576611641acde15c2322228d138258f236d14b749ad9af498ab69089e2d"},
+    {url = "https://files.pythonhosted.org/packages/cb/27/3946af83cd5911b1a5c3d987c0518f16b97ee4ccfeba90c6085e80bf35e4/pandas-2.0.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a6b5f14cd24a2ed06e14255ff40fe2ea0cfaef79a8dd68069b7ace74bd6acbba"},
+    {url = "https://files.pythonhosted.org/packages/cb/3f/4569dd34e3b77ad98e8532a43ca72fd332d4834a20b44efd7a979e6b23b5/pandas-2.0.2-cp39-cp39-win32.whl", hash = "sha256:598e9020d85a8cdbaa1815eb325a91cfff2bb2b23c1442549b8a3668e36f0f77"},
+    {url = "https://files.pythonhosted.org/packages/e8/1d/9ee861bea351b6bc4d025ac9edbc765bac11239188561ebc3cf032d930fb/pandas-2.0.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50e451932b3011b61d2961b4185382c92cc8c6ee4658dcd4f320687bb2d000ee"},
+    {url = "https://files.pythonhosted.org/packages/ee/fd/a3b5f229e5098e18cb058549f9c2842f407023adb47aa6b22b44b15988c6/pandas-2.0.2-cp311-cp311-win_amd64.whl", hash = "sha256:c4af689352c4fe3d75b2834933ee9d0ccdbf5d7a8a7264f0ce9524e877820c08"},
+    {url = "https://files.pythonhosted.org/packages/ef/e3/1b7a8d5a50b087bfc8b74245019943b33003f0b6fd28ccd63faf8825ea7e/pandas-2.0.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a18e5c72b989ff0f7197707ceddc99828320d0ca22ab50dd1b9e37db45b010c0"},
+    {url = "https://files.pythonhosted.org/packages/f0/95/361d9726b57b44c1d8dce070930c2322a70157f697ecdcca13f4388247ab/pandas-2.0.2-cp38-cp38-win_amd64.whl", hash = "sha256:e69140bc2d29a8556f55445c15f5794490852af3de0f609a24003ef174528b79"},
+    {url = "https://files.pythonhosted.org/packages/f2/36/27bbaf60ab48617024a00e2cae1211d58cee0557a457d7cc8933a05f01e8/pandas-2.0.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:713f2f70abcdade1ddd68fc91577cb090b3544b07ceba78a12f799355a13ee44"},
+    {url = "https://files.pythonhosted.org/packages/fb/88/d04926998a33223dbee6856970c5a7fd3cc83ded1f8782ccea8741ebd659/pandas-2.0.2.tar.gz", hash = "sha256:dd5476b6c3fe410ee95926873f377b856dbc4e81a9c605a0dc05aaccc6a7c6c6"},
 ]
 "parso 0.8.3" = [
     {url = "https://files.pythonhosted.org/packages/05/63/8011bd08a4111858f79d2b09aad86638490d62fbf881c44e434a6dfca87b/parso-0.8.3-py2.py3-none-any.whl", hash = "sha256:c001d4636cd3aecdaf33cbb40aebb59b094be2a74c556778ef5576c175e19e75"},
     {url = "https://files.pythonhosted.org/packages/a2/0e/41f0cca4b85a6ea74d66d2226a7cda8e41206a624f5b330b958ef48e2e52/parso-0.8.3.tar.gz", hash = "sha256:8c07be290bb59f03588915921e29e8a50002acaf2cdc5fa0e0114f91709fafa0"},
 ]
 "pathspec 0.11.1" = [
     {url = "https://files.pythonhosted.org/packages/95/60/d93628975242cc515ab2b8f5b2fc831d8be2eff32f5a1be4776d49305d13/pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
```

### Comparing `xklb-1.29.2/readme.py` & `xklb-1.29.3/readme.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,57 @@
-from xklb import lb, play_actions
-from xklb.scripts.scatter import scatter_usage
+from xklb import lb, usage
+
+usage_details = []
+for title, subcommand in [
+    ("Add local media", "fsadd"),
+    ("Add online media", "tubeadd"),
+    ("Add reddit media", "redditadd"),
+    ("Create / Update a Hacker News database", "hnadd"),
+    ("Add tabs", "tabsadd"),
+    ("Watch / Listen", "watch"),
+    ("Search captions / subtitles", "search"),
+    ("Open tabs", "tabs"),
+    ("Download media", "download"),
+    ("Show Download Status", "dlstatus"),
+    ("Update local media", "fsupdate"),
+    ("Update online media", "tubeupdate"),
+    ("Update reddit media", "redditupdate"),
+    ("Convert pushshift data to reddit.db format", "pushshift"),
+    ("List playlists", "playlists"),
+    ("Blocklist a channel", "block"),
+    ("Show large folders", "bigdirs"),
+    ("Copy play history", "copy-play-counts"),
+    ("Dedupe music", "dedupe"),
+    ("Re-optimize database", "optimize"),
+    ("Re-download media", "redownload"),
+    ("Merge online and local data", "merge-online-local"),
+    ("Convert selftext links to media table", "reddit-selftext"),
+    ("Merge SQLITE databases", "merge-dbs"),
+    ("Sort lines by similarity", "cluster-sort"),
+    ("Move files preserving parent folder hierarchy", "relmv"),
+    ("Automatic tab loader", "surf"),
+    ("Clean filenames", "christen"),
+    # scatter usage is already in readme so intentionally skipped here
+]:
+    if subcommand not in title.lower():
+        title += f" ({subcommand})"
+    usage_details.append(
+        f"""
+<details><summary>{title}</summary>
+
+    $ library {subcommand} -h
+    usage: {getattr(usage, subcommand.replace('-','_'))}
+
+</details>
+"""
+    )
+
+expand_all_js = """```js
+(() => { const readmeDiv = document.getElementById("readme"); const detailsElements = readmeDiv.getElementsByTagName("details"); for (let i = 0; i < detailsElements.length; i++) { detailsElements[i].setAttribute("open", "true"); } })();
+```"""
 
 print(
     rf"""# xk media library
 
 A wise philosopher once told me: "the future is [autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
 Manage and curate large media libraries. An index for your archive.
@@ -82,20 +130,22 @@
 
 ### 2. Watch / Listen from websites
 
     library watch maker.db
 
 To stop playing press Ctrl+C in either the terminal or mpv
 
-## Getting started with tabs: visit websites on a schedule
+</details>
+
+<details><summary>Tabs: visit websites on a schedule</summary>
 
-tabs is a way to organize your visits to URLs that you want to visit every once in a while.
+`tabs` is a way to organize your visits to URLs that you want to remember every once in a while.
 
-If you want to track _changes_ to websites over time there are better tools out there, like
-`huginn`, `urlwatch`, or `changedetection.io`.
+The main benefit of tabs is that you can have a large amount of tabs saved (say 500 monthly tabs) and only the smallest
+amount of tabs to satisfy that goal (500/30) tabs will open each day. 17 tabs per day seems manageable--500 all at once does not.
 
 The use-case of tabs are websites that you know are going to change: subreddits, games,
 or tools that you want to use for a few minutes daily, weekly, monthly, quarterly, or yearly.
 
 ### 1. Add your websites
 
     library tabsadd tabs.db --frequency monthly --category fun \
@@ -134,14 +184,16 @@
     systemctl --user daemon-reload
     systemctl --user enable --now tabs.service
 
 You can also invoke tabs manually:
 
     library tabs tabs.db -L 1  # open one tab
 
+Incremental surfing. 📈🏄 totally rad!
+
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
     {lb.usage()}
 
@@ -160,33 +212,27 @@
     library listen music.tl.db -ct "House speakers"
 
 ### Hook into HackerNews
 
     wget https://github.com/chapmanjacobd/hn_mining/raw/main/hackernews_only_direct.tw.db
     library watch hackernews_only_direct.tw.db --random --ignore-errors
 
-## Watch/Listen Usage
-
-    $ library watch -h
-    usage: {play_actions.usage('watch')}
-
-## More examples
-
 ### Organize via separate databases.
 
     library fsadd --audio both.db ./audiobooks/ ./podcasts/
     library fsadd --audio audiobooks.db ./audiobooks/
     library fsadd --audio podcasts.db ./podcasts/ ./another/more/secret/podcasts_folder/
 
 
 ### Find large folders to curate
 
 <details><summary>lb bigdirs</summary>
 
-Also, if you are just looking for folders which are candidates for curation (ie. I need space but don't want to buy a hard drive). The bigdirs subcommand was written for that purpose:
+If you are looking for candidate folders for curation (ie. you need space but don't want to buy another hard drive).
+The bigdirs subcommand was written for that purpose:
 
     $ lb bigdirs fs/d.db
 
 You may filter by folder depth (similar to QDirStat or WizTree)
 
     $ lb bigdirs --depth=3 audio.db
 
@@ -259,15 +305,15 @@
 
 
 ### Scatter your data across disks with [mergerfs](https://github.com/trapexit/mergerfs)
 
 <details><summary>If you use mergerfs, you'll likely be interested in this</summary>
 
     library scatter -h
-    usage: {scatter_usage}
+    usage: {usage.scatter}
 
     positional arguments:
     database
     relative_paths        Paths to scatter, relative to the root of your mergerfs mount; any path substring is valid
 
     options:
     -h, --help            show this help message and exit
@@ -395,9 +441,17 @@
 ### Datasette
 
 Explore `library` databases in your browser
 
     pip install datasette
     datasette tv.db
 
+## Usage
+
+{''.join(usage_details)}
+
+You can expand all by running this in your browser console:
+
+{expand_all_js}
+
 """,
 )
```

### Comparing `xklb-1.29.2/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.29.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.29.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/.github/workflows/push.yaml` & `xklb-1.29.3/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/sql/transfer.sql` & `xklb-1.29.3/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/av.py` & `xklb-1.29.3/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/books.py` & `xklb-1.29.3/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/consts.py` & `xklb-1.29.3/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/db.py` & `xklb-1.29.3/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/dl_config.py` & `xklb-1.29.3/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/fs_extract.py` & `xklb-1.29.3/xklb/fs_extract.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import partial
 from multiprocessing import TimeoutError as mp_TimeoutError
 from pathlib import Path
 from shutil import which
 from timeit import default_timer as timer
 from typing import Dict, List, Optional
 
-from xklb import av, books, consts, db, player, utils
+from xklb import av, books, consts, db, player, usage, utils
 from xklb.consts import SC, DBType
 from xklb.utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
 
@@ -381,80 +381,24 @@
         db.optimize(args)
 
 
 def fs_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args = parse_args(
-        SC.fsadd,
-        """library fsadd [--audio | --video | --image |  --text | --filesystem] -c CATEGORY [database] paths ...
-
-    The default database type is video:
-        library fsadd tv.db ./tv/
-        library fsadd --video tv.db ./tv/  # equivalent
-
-    You can also create audio databases. Both audio and video use ffmpeg to read metadata:
-        library fsadd --audio audio.db ./music/
-
-    Image uses ExifTool:
-        library fsadd --image image.db ./photos/
-
-    Text will try to read files and save the contents into a searchable database:
-        library fsadd --text text.db ./documents_and_books/
-
-    Create a text database and scan with OCR and speech-recognition:
-        library fsadd --text --ocr --speech-recognition ocr.db ./receipts_and_messages/
-
-    Create a video database and read internal/external subtitle files into a searchable database:
-        library fsadd --scan-subtitles tv.search.db ./tv/ ./movies/
-
-    Decode media to check for corruption (slow):
-        library fsadd --check-corrupt 100 tv.db ./tv/  # scan through 100 percent of each file to evaluate how corrupt it is (very slow)
-        library fsadd --check-corrupt   1 tv.db ./tv/  # scan through 1 percent of each file to evaluate how corrupt it is (takes about one second per file)
-        library fsadd --check-corrupt   5 tv.db ./tv/  # scan through 1 percent of each file to evaluate how corrupt it is (takes about ten seconds per file)
-
-        library fsadd --check-corrupt   5 --delete-corrupt 30 tv.db ./tv/  # scan 5 percent of each file to evaluate how corrupt it is, if 30 percent or more of those checks fail then the file is deleted
-
-        nb: the behavior of delete-corrupt changes between full and partial scan
-        library fsadd --check-corrupt  99 --delete-corrupt  1 tv.db ./tv/  # partial scan 99 percent of each file to evaluate how corrupt it is, if 1 percent or more of those checks fail then the file is deleted
-        library fsadd --check-corrupt 100 --delete-corrupt  1 tv.db ./tv/  # full scan each file to evaluate how corrupt it is, if there is _any_ corruption then the file is deleted
-
-    Normally only relevant filetypes are included. You can scan all files with this flag:
-        library fsadd --scan-all-files mixed.db ./tv-and-maybe-audio-only-files/
-        # I use that with this to keep my folders organized:
-        library watch -w 'video_count=0 and audio_count>=1' -pf mixed.db | parallel mv {} ~/d/82_Audiobooks/
-
-    Remove path roots with --force
-        library fsadd audio.db /mnt/d/Youtube/
-        [/mnt/d/Youtube] Path does not exist
-
-        library fsadd --force audio.db /mnt/d/Youtube/
-        [/mnt/d/Youtube] Path does not exist
-        [/mnt/d/Youtube] Building file list...
-        [/mnt/d/Youtube] Marking 28932 orphaned metadata records as deleted
-    """,
-    )
+    args = parse_args(SC.fsadd, usage.fsadd)
 
     extractor(args, args.paths)
 
 
 def fs_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args = parse_args(
-        SC.fsupdate,
-        """library fsupdate database
-
-    Update each path previously saved:
-
-        library fsupdate database
-    """,
-    )
+    args = parse_args(SC.fsupdate, usage.fsupdate)
 
     playlists = list(
         args.db.query(
             """
             SELECT *
             FROM playlists
             WHERE ie_key = 'Local'
```

### Comparing `xklb-1.29.2/xklb/gui.py` & `xklb-1.29.3/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/hn_extract.py` & `xklb-1.29.3/xklb/hn_extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse, asyncio, queue, sqlite3, threading
 from pathlib import Path
 
-from xklb import db, utils
+from xklb import db, usage, utils
 from xklb.utils import log
 
 """
 My understanding of aiohttp is stolen
 from ashish01's excellent https://github.com/ashish01/hn-data-dumps/blob/main/hn_async2.py
 
 MIT License
@@ -109,32 +109,15 @@
             task.add_done_callback(background_tasks.discard)
 
         for _i in range(N):
             await sem.acquire()
 
 
 def hacker_news_add() -> None:
-    args = parse_args(
-        prog="library hnadd",
-        usage="""library hnadd [--oldest] database
-
-    Fetch latest stories first:
-
-        library hnadd hn.db -v
-        Fetching 154873 items (33212696 to 33367569)
-        Saving comment 33367568
-        Saving comment 33367543
-        Saving comment 33367564
-        ...
-
-    Fetch oldest stories first:
-
-        library hnadd --oldest hn.db
-    """,
-    )
+    args = parse_args(prog="library hnadd", usage=usage.hnadd)
     try:
         import aiohttp
     except ModuleNotFoundError:
         log.error("aiohttp is required for hn_extract. Install with pip install aiohttp or pip install xklb[full]")
         raise
 
     args.db.enable_wal()
```

### Comparing `xklb-1.29.2/xklb/lb.py` & `xklb-1.29.3/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/playback.py` & `xklb-1.29.3/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/player.py` & `xklb-1.29.3/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/praw_extract.py` & `xklb-1.29.3/xklb/praw_extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import sys
 from functools import partial
 from itertools import takewhile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple
 
-from xklb import consts, db, utils
+from xklb import consts, db, usage, utils
 from xklb.utils import log
 
 PRAW_SETUP_INSTRUCTIONS = r"""
 You will need your Reddit user login info, client id, and secret.
 See https://www.reddit.com/wiki/api for client id / secret.
 
 Then create a praw.ini file:
@@ -338,31 +338,15 @@
             continue
 
 
 def reddit_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args = parse_args(
-        "redditadd",
-        usage="""library redditadd [--lookback N_DAYS] [--praw-site bot1] [database] paths ...
-
-    Fetch data for redditors and reddits:
-
-        library redditadd https://old.reddit.com/r/coolgithubprojects/ https://old.reddit.com/user/Diastro
-
-    If you have a file with a list of subreddits you can do this:
-
-        library redditadd --subreddits --db 96_Weird_History.db (cat ~/mc/96_Weird_History-reddit.txt)
-
-    Likewise for redditors:
-
-        library redditadd --redditors --db idk.db (cat ~/mc/shadow_banned.txt)
-    """,
-    )
+    args = parse_args("redditadd", usage=usage.redditadd)
 
     subreddits = []
     redditors = []
     for path in args.paths:
         subreddit_matches = consts.REGEX_SUBREDDIT.match(path)
         redditor_matches = consts.REGEX_REDDITOR.match(path)
         ie_key = "reddit_praw"
@@ -410,23 +394,15 @@
         db.optimize(args)
 
 
 def reddit_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args = parse_args(
-        "redditupdate",
-        usage="""library redditupdate [--audio | --video] [-c CATEGORY] [--lookback N_DAYS] [--praw-site bot1] [database]
-
-    Fetch the latest posts for every subreddit/redditor saved in your database
-
-        library redditupdate edu_subreddits.db
-    """,
-    )
+    args = parse_args("redditupdate", usage=usage.redditupdate)
     playlists = db.get_playlists(
         args,
         "ie_key, path, id, config",
         sql_filters=['AND ie_key in ("reddit_praw_subreddit","reddit_praw_redditor")'],
         constrain=True,
     )
```

### Comparing `xklb-1.29.2/xklb/search.py` & `xklb-1.29.3/xklb/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,20 @@
 import argparse, json, textwrap
 from copy import deepcopy
 from itertools import groupby
 from typing import Tuple
 
 from tabulate import tabulate
 
-from xklb import consts, db, player, utils
+from xklb import consts, db, player, usage, utils
 from xklb.utils import log, pipe_print
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
-        prog="library search",
-        usage="""library search
-
-    Search text databases and subtitles
-
-    $ library search fts.db boil
-        7 captions
-        /mnt/d/70_Now_Watching/DidubeTheLastStop-720p.mp4
-           33:46 I brought a real stainless steel boiler
-           33:59 The world is using only stainless boilers nowadays
-           34:02 The boiler is old and authentic
-           34:30 - This boiler? - Yes
-           34:44 I am not forcing you to buy this boiler…
-           34:52 Who will give her a one liter stainless steel boiler for one Lari?
-           34:54 Glass boilers cost two
-
-    Search and open file
-    $ library search fts.db dashi --open
-""",
-    )
+    parser = argparse.ArgumentParser(prog="library search", usage=usage.search)
     parser.add_argument("--open", "--play", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
     parser.add_argument("--overlap", type=int, default=8, help=argparse.SUPPRESS)
     parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--sort", "-u", nargs="+", default=["path", "time"], help=argparse.SUPPRESS)
@@ -161,32 +141,32 @@
         return caption["time"] + (len(caption["text"]) / 4.2 / 220 * 60)
 
     merged_captions = []
     for path, group in groupby(
         captions, key=lambda x: x["path"]
     ):  # group by only does contiguous items with the same key
         group = list(group)
-        merged_group = {"path": path, "time": group[0]["time"], "end": get_end(group[0]), "text": group[0]["text"]}
+        merged_group = {"path": path, "time": group[0]["time"], "end": get_end(group[0]), "text": group[0]["text"]}  # type: ignore
         for i in range(1, len(group)):
             end = get_end(group[i])
 
             if (
-                abs(group[i]["time"] - merged_group["end"]) <= args.overlap
-                or abs(group[i]["time"] - merged_group["time"]) <= args.overlap
+                abs(group[i]["time"] - merged_group["end"]) <= args.overlap  # type: ignore
+                or abs(group[i]["time"] - merged_group["time"]) <= args.overlap  # type: ignore
             ):
                 merged_group["end"] = end
-                if group[i]["text"] not in merged_group["text"]:
-                    merged_group["text"] += ". " + group[i]["text"]
+                if group[i]["text"] not in merged_group["text"]:  # type: ignore
+                    merged_group["text"] += ". " + group[i]["text"]  # type: ignore
             else:
                 merged_captions.append(merged_group)
                 merged_group = {
                     "path": path,
-                    "time": group[i]["time"],
+                    "time": group[i]["time"],  # type: ignore
                     "end": end,
-                    "text": group[i]["text"],
+                    "text": group[i]["text"],  # type: ignore
                 }
         merged_captions.append(merged_group)
 
     return merged_captions
 
 
 def search() -> None:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xklb-1.29.2/xklb/subtitle.py` & `xklb-1.29.3/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/tube_backend.py` & `xklb-1.29.3/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/tube_extract.py` & `xklb-1.29.3/xklb/tabs_actions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,176 +1,184 @@
-import argparse, sys
+import argparse
 from pathlib import Path
+from time import sleep
+from typing import Dict, List, Tuple
 
-from xklb import db, tube_backend, utils
+from xklb import db, usage, utils
 from xklb.consts import SC
-from xklb.utils import log
+from xklb.player import generic_player, mark_media_watched, override_sort, printer
+from xklb.tabs_extract import Frequency
+from xklb.utils import cmd, flatten, log
 
 
-def parse_args(action, usage) -> argparse.Namespace:
+def parse_args(action) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        prog="library " + action,
-        usage=usage,
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        prog="library tabs", formatter_class=argparse.ArgumentDefaultsHelpFormatter, usage=usage.tabs
     )
 
-    parser.add_argument(
-        "--dl-config",
-        "-dl-config",
-        nargs=1,
-        action=utils.ArgparseDict,
-        default={},
-        metavar="KEY=VALUE",
-        help="Add key/value pairs to override or extend default downloader configuration",
-    )
-    parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
-    parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
-    parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
-    parser.add_argument("--extra", "-extra", action="store_true", help="Get full metadata (takes a lot longer)")
-    parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
-    parser.add_argument("--playlist-db", action="store_true", help="Fetch metadata for paths in a table")
-    parser.add_argument("--subs", action="store_true")
-    parser.add_argument("--auto-subs", "--autosubs", action="store_true")
-    parser.add_argument("--subtitle-languages", "--subtitle-language", "--slang", "--lang", action="extend", nargs="+")
-    parser.add_argument("--extra-media-data", default={})
-    parser.add_argument("--extra-playlist-data", default={})
-    parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", "-f", action="store_true", help=argparse.SUPPRESS)
-
-    if action in (SC.tubeadd, SC.tubeupdate):
-        parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
+    parser.add_argument("--sort", "-u", nargs="+")
+    parser.add_argument("--where", "-w", nargs="+", action="extend", default=[])
+    parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[])
+    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[])
+    parser.add_argument("--print", "-p", default=False, const="p", nargs="?")
+    parser.add_argument("--delete", "--remove", "--erase", "--rm", "-rm", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--cols", "-cols", "-col", nargs="*", help="Include a non-standard column when printing")
+    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue")
+    parser.add_argument("--skip")
 
-    parser.add_argument("--timeout", "-T", help="Quit after x minutes")
+    parser.add_argument("--db", "-db")
     parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
-    if action == SC.tubeadd:
-        parser.add_argument("playlists", nargs="+", help=argparse.SUPPRESS)
-
-    args = parser.parse_args()
+    parser.add_argument("search", nargs="*")
+    args = parser.parse_intermixed_args()
     args.action = action
 
+    args.include += args.search
+    if args.include == ["."]:
+        args.include = [str(Path().cwd().resolve())]
+
     if args.db:
         args.database = args.db
-    if action == SC.tubeadd:
-        Path(args.database).touch()
-    args.db = db.connect(args)
-
-    if hasattr(args, "no_sanitize") and hasattr(args, "playlists") and not args.no_sanitize:
-        args.playlists = [utils.sanitize_url(args, p) for p in args.playlists]
-    if hasattr(args, "playlists"):
-        args.playlists = utils.conform(args.playlists)
-    log.info(utils.dict_filter_bool(args.__dict__))
-
-    utils.timeout(args.timeout)
-
-    return args
-
-
-def tube_add(args=None) -> None:
-    if args:
-        sys.argv = ["tubeadd", *args]
-
-    args = parse_args(
-        SC.tubeadd,
-        usage=r"""library tubeadd [--audio | --video] -c CATEGORY [database] playlists ...
 
-    Create a dl database / add links to an existing database
+    if args.sort:
+        args.sort = [override_sort(s) for s in args.sort]
+        args.sort = " ".join(args.sort)
 
-        library tubeadd -c Educational dl.db https://www.youdl.com/c/BranchEducation/videos
+    if args.cols:
+        args.cols = list(flatten([s.split(",") for s in args.cols]))
 
-    Add metadata for links in a database table
+    if args.delete:
+        args.print += "d"
 
-        library tubeadd reddit.db --playlist-db media
-
-    If you include more than one URL, you must specify the database
-
-        library tubeadd 71_Mealtime_Videos dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
-
-    Files will be saved to <lb download prefix>/<lb tubeadd category>/
-
-        For example:
-        library tubeadd Cool ...
-        library download D:\'My Documents'\ ...
-        Media will be downloaded to 'D:\My Documents\Cool\'
-
-    Fetch extra metadata:
-
-        By default tubeadd will quickly add media at the expense of less metadata.
-        If you plan on using `library download` then it doesn't make sense to use `--extra`.
-        Downloading will add the extra metadata automatically to the database.
-        You can always fetch more metadata later via tubeupdate:
-        library tubeupdate tw.db --extra
-    """,
-    )
-    if args.playlist_files:
-        args.playlists = list(utils.flatten([Path(p).read_text().splitlines() for p in args.playlists]))
-    elif args.playlist_db:
-        args.playlists = list(
-            utils.flatten(
-                [
-                    d["path"]
-                    for d in args.db.query(
-                        f"""
-                    select path from {table}
-                    where 1=1
-                    and COALESCE(time_deleted,0) = 0
-                    and COALESCE(time_modified,0) = 0
-                    and COALESCE(time_downloaded,0) = 0
-                    {'and width is null' if 'width' in args.db[table].columns_dict else ''}
-                    {'and title is null' if 'title' in args.db[table].columns_dict else ''}
-                    {'and duration is null' if 'duration' in args.db[table].columns_dict else ''}
-                    {'and size is null' if 'size' in args.db[table].columns_dict else ''}
-                    ORDER by random()
-                    """,
-                    )
-                ]
-                for table in args.playlists
-            ),
-        )
-
-    for path in args.playlists:
-        if args.safe and not tube_backend.is_supported(path):
-            log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
-            continue
-
-        tube_backend.process_playlist(args, path, tube_backend.tube_opts(args))
-
-        if args.extra:
-            log.warning("[%s]: Getting extra metadata", path)
-            tube_backend.get_extra_metadata(args, path)
-
-    LARGE_NUMBER = 100_000
-    if not args.db["media"].detect_fts() or tube_backend.added_media_count > LARGE_NUMBER:
-        db.optimize(args)
-
-
-def tube_update(args=None) -> None:
-    if args:
-        sys.argv = ["tubeupdate", *args]
-
-    args = parse_args(
-        SC.tubeupdate,
-        usage="""library tubeupdate [--audio | --video] [-c CATEGORY] [database]
-
-    Fetch the latest videos for every playlist saved in your database
-
-        library tubeupdate educational.db
-
-    Or limit to specific categories...
-
-        library tubeupdate -c "Bob Ross" educational.db
-
-    Run with --optimize to add indexes (might speed up searching but the size will increase):
-
-        library tubeupdate --optimize examples/music.tl.db
+    if args.db:
+        args.database = args.db
+    args.db = db.connect(args)
+    log.info(utils.dict_filter_bool(args.__dict__))
 
-    Fetch extra metadata:
+    return args
 
-        By default tubeupdate will quickly add media.
-        You can run with --extra to fetch more details: (best resolution width, height, subtitle tags, etc)
 
-        library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
-""",
-    )
-    playlists = db.get_playlists(args, constrain=True)
-    tube_backend.update_playlists(args, playlists)
+def tabs_include_sql(x) -> str:
+    return f"""and (
+    path like :include{x}
+    OR category like :include{x}
+    OR frequency like :include{x}
+)"""
+
+
+def tabs_exclude_sql(x) -> str:
+    return f"""and (
+    path not like :exclude{x}
+    AND category not like :exclude{x}
+    AND frequency not like :exclude{x}
+)"""
+
+
+def construct_tabs_query(args) -> Tuple[str, dict]:
+    args.filter_sql = []
+    args.filter_bindings = {}
+
+    args.filter_sql.extend([" and " + w for w in args.where])
+
+    for idx, inc in enumerate(args.include):
+        args.filter_sql.append(tabs_include_sql(idx))
+        args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
+    for idx, exc in enumerate(args.exclude):
+        args.filter_sql.append(tabs_exclude_sql(idx))
+        args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
+
+    LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
+    OFFSET = f"OFFSET {args.skip}" if args.skip else ""
+
+    query = f"""SELECT path
+        , frequency
+        , CASE
+            WHEN frequency = 'daily' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+1 Day' )) as int)
+            WHEN frequency = 'weekly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+7 Days' )) as int)
+            WHEN frequency = 'monthly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+1 Month' )) as int)
+            WHEN frequency = 'quarterly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+3 Months' )) as int)
+            WHEN frequency = 'yearly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+1 Year' )) as int)
+        END time_valid
+        {', ' + ', '.join(args.cols) if args.cols else ''}
+    FROM media
+    WHERE 1=1
+        and COALESCE(time_deleted,0) = 0
+        {" ".join(args.filter_sql)}
+        {"and time_valid < cast(STRFTIME('%s', datetime()) as int)" if not args.print else ''}
+    ORDER BY 1=1
+        {', ' + args.sort if args.sort else ''}
+        {', time_played, time_valid, path' if args.print else ''}
+        , play_count
+        , frequency = 'daily' desc
+        , frequency = 'weekly' desc
+        , frequency = 'monthly' desc
+        , frequency = 'quarterly' desc
+        , frequency = 'yearly' desc
+        , ROW_NUMBER() OVER ( PARTITION BY
+            play_count
+            , frequency
+            , hostname
+            , category
+        ) -- prefer to spread hostname, category over time
+        , random()
+    {LIMIT} {OFFSET}
+    """
+
+    return query, args.filter_bindings
+
+
+def play(args, m: Dict) -> None:
+    media_file = m["path"]
+
+    cmd(*generic_player(args), media_file, strict=False)
+    mark_media_watched(args, [media_file])
+
+
+def frequency_filter(args, media: List[Dict]) -> List[dict]:
+    mapper = {
+        Frequency.Daily.value: 1,
+        Frequency.Weekly.value: 7,
+        Frequency.Monthly.value: 30,
+        Frequency.Quarterly.value: 91,
+        Frequency.Yearly.value: 365,
+    }
+    counts = args.db.execute("select frequency, count(*) from media group by 1").fetchall()
+    filtered_media = []
+    for freq, freq_count in counts:
+        num_days = mapper.get(freq, 365)
+        num_tabs = max(1, freq_count // num_days)
+        log.debug(f"freq_count {freq_count} // num_days {num_days} = num_tabs {num_tabs}")
+
+        t = []
+        for m in media:
+            if m["frequency"] == freq:
+                t.append(m)
+
+        filtered_media.extend(t[:num_tabs])
+
+    return filtered_media
+
+
+def process_tabs_actions(args) -> None:
+    query, bindings = construct_tabs_query(args)
+
+    if args.print:
+        return printer(args, query, bindings)
+
+    media = list(args.db.query(query, bindings))
+    if not media:
+        utils.no_media_found()
+
+    media = frequency_filter(args, media)
+
+    for m in media:
+        play(args, m)
+        MANY_TABS = 9
+        if len(media) >= MANY_TABS:
+            sleep(0.3)
+    return None
+
+
+def tabs() -> None:
+    args = parse_args(SC.tabs)
+    process_tabs_actions(args)
```

### Comparing `xklb-1.29.2/xklb/utils.py` & `xklb-1.29.3/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/scripts/bigdirs.py` & `xklb-1.29.3/xklb/scripts/bigdirs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 import argparse
 from pathlib import Path
 from typing import Dict, List
 
 from tabulate import tabulate
 
-from xklb import db, utils
+from xklb import db, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library bigdirs",
-        usage="""library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by "deleted" | "played"] [--size=+5MB]
-
-    See what folders take up space
-
-        lb bigdirs video.db
-        lb bigdirs audio.db
-        lb bigdirs fs.db
-""",
+        usage=usage.bigdirs,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--sort-by")
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="4000")
     parser.add_argument("--depth", "-d", default=0, type=int, help="Depth of folders")
     parser.add_argument("--lower", type=int, help="Number of files per folder lower limit")
     parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
```

### Comparing `xklb-1.29.2/xklb/scripts/christen.py` & `xklb-1.29.3/xklb/scripts/christen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,17 @@
 import argparse, shutil
 from os import fsdecode
 from pathlib import Path
 
-from xklb import utils
+from xklb import usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
-        prog="library christen",
-        usage="""library christen DATABASE [--run]
-
-    Rename files to be somewhat normalized
-
-    Default mode is dry-run
-
-        lb christen fs.db
-
-    To actually do stuff use the run flag
-
-        lb christen audio.db --run
-
-    You can optionally replace all the spaces in your filenames with dots
-
-        lb christen --dot-space video.db
-""",
-    )
+    parser = argparse.ArgumentParser(prog="library christen", usage=usage.christen)
     parser.add_argument("paths", nargs="*")
     parser.add_argument("--dot-space", action="store_true")
     parser.add_argument("--overwrite", "-f", action="store_true")
     parser.add_argument("--run", "-r", action="store_true")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     args = parser.parse_args()
```

### Comparing `xklb-1.29.2/xklb/scripts/cluster_sort.py` & `xklb-1.29.3/xklb/scripts/cluster_sort.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import argparse, sys
 
-from xklb import utils
+from xklb import usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
-        prog="library cluster-sort",
-        usage="""library cluster-sort [input_path | stdin] [output_path | stdout]
-
-    Group lines of text into sorted output
-""",
-    )
+    parser = argparse.ArgumentParser(prog="library cluster-sort", usage=usage.cluster_sort)
     parser.add_argument("--model", "-m", help="Use a specific spaCy model")
     parser.add_argument("--clusters", "--n-clusters", "-c", type=int, help="Number of KMeans clusters")
     parser.add_argument("--groups", "-g", action="store_true", help="Show groups")
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
     parser.add_argument("input_path", nargs="?", type=argparse.FileType("r"), default=sys.stdin)
     parser.add_argument("output_path", nargs="?")
```

### Comparing `xklb-1.29.2/xklb/scripts/copy_play_counts.py` & `xklb-1.29.3/xklb/scripts/copy_play_counts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 import argparse
 from pathlib import Path
 
-from xklb import db, utils
+from xklb import db, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
-        prog="library copy-play-counts",
-        usage="""library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
-
-    Copy play count information between databases
-
-        lb copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
-""",
-    )
+    parser = argparse.ArgumentParser(prog="library copy-play-counts", usage=usage.copy_play_counts)
     parser.add_argument("database")
     parser.add_argument("source_dbs", nargs="+")
     parser.add_argument("--source-prefix", default="")
     parser.add_argument("--target-prefix", default="")
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
     args = parser.parse_intermixed_args()
```

### Comparing `xklb-1.29.2/xklb/scripts/dedupe.py` & `xklb-1.29.3/xklb/scripts/dedupe.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,21 @@
 from copy import deepcopy
 from pathlib import Path
 from typing import List
 
 import humanize
 from tabulate import tabulate
 
-from xklb import db, player, utils
+from xklb import db, player, usage, utils
 from xklb.consts import DBType
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
-        prog="library dedupe",
-        usage="""library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
-
-    Dedupe your files
-""",
-    )
+    parser = argparse.ArgumentParser(prog="library dedupe", usage=usage.dedupe)
 
     profile = parser.add_mutually_exclusive_group()
     profile.add_argument(
         "--audio",
         action="store_const",
         dest="profile",
         const=DBType.audio,
```

### Comparing `xklb-1.29.2/xklb/scripts/merge_online_local.py` & `xklb-1.29.3/xklb/scripts/merge_online_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 import argparse
 from copy import deepcopy
 from typing import List, Optional
 
 from tabulate import tabulate
 
-from xklb import consts, db, utils
+from xklb import consts, db, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
-        prog="library merge-online-local",
-        usage="""library merge-online-local DATABASE
-
-    If you have previously downloaded YouTube or other online media, you can dedupe
-    your database and combine the online and local media records as long as your
-    files have the youtube-dl / yt-dlp id in the filename.
-    """,
-    )
+    parser = argparse.ArgumentParser(prog="library merge-online-local", usage=usage.merge_online_local)
     parser.add_argument("database")
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default=100)
     parser.add_argument("--verbose", "-v", action="count", default=0)
     args = parser.parse_args()
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
```

### Comparing `xklb-1.29.2/xklb/scripts/move_list.py` & `xklb-1.29.3/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/scripts/optimize_db.py` & `xklb-1.29.3/xklb/scripts/optimize_db.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 import argparse
 
-from xklb import db, utils
+from xklb import db, usage, utils
 from xklb.utils import log
 
 
 def optimize_db() -> None:
-    parser = argparse.ArgumentParser(
-        prog="library optimize",
-        usage="""library optimize DATABASE [--force]
-
-    Optimize library databases
-
-    The force flag is usually unnecessary and it can take much longer
-""",
-    )
+    parser = argparse.ArgumentParser(prog="library optimize", usage=usage.optimize)
     parser.add_argument("--force", "-f", action="store_true")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
     parser.add_argument("database")
     args = parser.parse_args()
     if args.db:
         args.database = args.db
```

### Comparing `xklb-1.29.2/xklb/scripts/relmv.py` & `xklb-1.29.3/xklb/scripts/relmv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 import argparse, shlex
 from collections import OrderedDict
 from os.path import commonprefix
 from pathlib import Path
 
-from xklb import utils
+from xklb import usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
-        prog="library relmv",
-        usage="""library relmv [--dry-run] SOURCE ... DEST
-
-    Move files/folders without losing hierarchy metadata
-
-    Move fresh music to your phone every Sunday:
-
-        # move last weeks' music back to their source folders
-        lb relmv /mnt/d/80_Now_Listening/ /mnt/d/
-
-        # move new music for this week
-        lb relmv (
-            lb listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
-        ) /mnt/d/80_Now_Listening/
-""",
-    )
+    parser = argparse.ArgumentParser(prog="library relmv", usage=usage.relmv)
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--test", "--dry-run", action="store_true")
 
     parser.add_argument("sources", nargs="+", help="one or more source files or directories to move")
     parser.add_argument("dest", help="destination directory")
     args = parser.parse_args()
```

### Comparing `xklb-1.29.2/xklb/scripts/streaming_tab_loader.py` & `xklb-1.29.3/xklb/scripts/streaming_tab_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 import argparse, logging, sys
 from time import sleep
 from typing import List
 
-from xklb import db, player, utils
+from xklb import db, player, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library surf",
-        usage="""library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
-
-    Streaming tab loader: press ctrl+c to stop.
-
-    Open tabs from a line-delimited file:
-
-        cat tabs.txt | library surf -n 5
-
-    You will likely want to use this setting in `about:config`
-
-        browser.tabs.loadDivertedInBackground = True
-
-    If you prefer GUI, check out https://unli.xyz/tabsender/
-    """,
+        usage=usage.surf,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("database")
     parser.add_argument("--count", "-n", default=2, type=int)
     parser.add_argument("--target-hosts", "--target", default=None, help="Target hosts IP:Port")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     args = parser.parse_args()
```

### Comparing `xklb-1.29.2/xklb/scripts/mining/data.py` & `xklb-1.29.3/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/scripts/mining/extract_links.py` & `xklb-1.29.3/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/scripts/mining/nouns.py` & `xklb-1.29.3/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/xklb/scripts/mining/pushshift.py` & `xklb-1.29.3/xklb/scripts/mining/pushshift.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse, sys
 from pathlib import Path
 
-from xklb import db, utils
+from xklb import db, usage, utils
 from xklb.praw_extract import slim_post_data
 from xklb.utils import log
 
 try:
     import orjson
 except ModuleNotFoundError:
     import json as orjson
@@ -38,34 +38,15 @@
         media.clear()
 
 
 def pushshift_extract(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args = parse_args(
-        "pushshift",
-        usage="""library pushshift [database] < stdin
-
-    Download data (about 600GB jsonl.zst; 6TB uncompressed)
-
-        wget -e robots=off -r -k -A zst https://files.pushshift.io/reddit/submissions/
-
-    Load data from files via unzstd
-
-        unzstd --memory=2048MB --stdout RS_2005-07.zst | library pushshift pushshift.db
-
-    Or multiple (output is about 1.5TB SQLITE fts-searchable):
-
-        for f in psaw/files.pushshift.io/reddit/submissions/*.zst
-            echo "unzstd --memory=2048MB --stdout $f | library pushshift (basename $f).db"
-            library optimize (basename $f).db
-        end | parallel -j5
-    """,
-    )
+    args = parse_args("pushshift", usage=usage.pushshift)
 
     args.db.enable_wal()
 
     count = 0
     reddit_posts = []
     media = []
     for line in sys.stdin:
```

### Comparing `xklb-1.29.2/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.29.3/xklb/scripts/mining/reddit_selftext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import argparse, html
 from typing import Set, Tuple
 from urllib.parse import urlparse
 
-from xklb import db, utils
+from xklb import db, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(
-        prog="library reddit-selftext",
-        usage="""library reddit-selftext DATABASE
-
-    Extract URLs from reddit selftext from the reddit_posts table to the media table
-""",
-    )
+    parser = argparse.ArgumentParser(prog="library reddit-selftext", usage=usage.reddit_selftext)
     parser.add_argument("database")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     args = parser.parse_args()
 
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
```

### Comparing `xklb-1.29.2/xklb/assets/kotobago.png` & `xklb-1.29.3/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/.gitignore` & `xklb-1.29.3/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/LICENSE` & `xklb-1.29.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/pyproject.toml` & `xklb-1.29.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.29.2/PKG-INFO` & `xklb-1.29.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,7 @@
-Metadata-Version: 2.1
-Name: xklb
-Version: 1.29.2
-Summary: xk library
-Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
-Project-URL: homepage, https://github.com/chapmanjacobd/library/
-Project-URL: repository, https://github.com/chapmanjacobd/library/
-Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
-License: BSD 3-Clause No Nuclear License
-        
-        Copyright (c) 2021, Jacob Chapman
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this
-          list of conditions and the following disclaimer.
-        
-        * Redistributions in binary form must reproduce the above copyright notice,
-          this list of conditions and the following disclaimer in the documentation
-          and/or other materials provided with the distribution.
-        
-        * Neither the name of the copyright holder nor the names of its
-          contributors may be used to endorse or promote products derived from
-          this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-        You acknowledge that this software is not designed nor intended for use in the
-        design, construction, operation or maintenance of any nuclear facility.
-License-File: LICENSE
-Requires-Python: >=3.8
-Requires-Dist: catt
-Requires-Dist: ffmpeg-python
-Requires-Dist: ftfy
-Requires-Dist: gallery-dl
-Requires-Dist: humanize
-Requires-Dist: ipython
-Requires-Dist: markdown
-Requires-Dist: mutagen
-Requires-Dist: natsort
-Requires-Dist: praw
-Requires-Dist: pysubs2
-Requires-Dist: python-mpv-jsonipc
-Requires-Dist: regex
-Requires-Dist: rich
-Requires-Dist: screeninfo
-Requires-Dist: sqlite-utils>=3.30
-Requires-Dist: subliminal
-Requires-Dist: tabulate
-Requires-Dist: tinytag
-Requires-Dist: yt-dlp
-Provides-Extra: all
-Requires-Dist: xklb[deluxe,dev,test]; extra == 'all'
-Provides-Extra: deluxe
-Requires-Dist: aiohttp; extra == 'deluxe'
-Requires-Dist: brotab; extra == 'deluxe'
-Requires-Dist: orjson; extra == 'deluxe'
-Requires-Dist: pandas; extra == 'deluxe'
-Requires-Dist: pyexiftool; extra == 'deluxe'
-Requires-Dist: sklearn; extra == 'deluxe'
-Requires-Dist: spacy; extra == 'deluxe'
-Requires-Dist: textract; extra == 'deluxe'
-Provides-Extra: dev
-Requires-Dist: black; extra == 'dev'
-Requires-Dist: ipdb; extra == 'dev'
-Requires-Dist: isort; extra == 'dev'
-Requires-Dist: scalene; extra == 'dev'
-Requires-Dist: ssort; extra == 'dev'
-Provides-Extra: test
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: ruff; extra == 'test'
-Description-Content-Type: text/markdown
-
 # xk media library
 
 A wise philosopher once told me: "the future is [autotainment](https://www.youtube.com/watch?v=F9sZFrsjPp0)".
 
 Manage and curate large media libraries. An index for your archive.
 Primary usage is local filesystem but also supports some virtual constructs like
 tracking online video playlists (eg. YouTube subscriptions) and scheduling browser tabs.
@@ -162,20 +78,22 @@
 
 ### 2. Watch / Listen from websites
 
     library watch maker.db
 
 To stop playing press Ctrl+C in either the terminal or mpv
 
-## Getting started with tabs: visit websites on a schedule
+</details>
+
+<details><summary>Tabs: visit websites on a schedule</summary>
 
-tabs is a way to organize your visits to URLs that you want to visit every once in a while.
+`tabs` is a way to organize your visits to URLs that you want to remember every once in a while.
 
-If you want to track _changes_ to websites over time there are better tools out there, like
-`huginn`, `urlwatch`, or `changedetection.io`.
+The main benefit of tabs is that you can have a large amount of tabs saved (say 500 monthly tabs) and only the smallest
+amount of tabs to satisfy that goal (500/30) tabs will open each day. 17 tabs per day seems manageable--500 all at once does not.
 
 The use-case of tabs are websites that you know are going to change: subreddits, games,
 or tools that you want to use for a few minutes daily, weekly, monthly, quarterly, or yearly.
 
 ### 1. Add your websites
 
     library tabsadd tabs.db --frequency monthly --category fun \
@@ -214,20 +132,22 @@
     systemctl --user daemon-reload
     systemctl --user enable --now tabs.service
 
 You can also invoke tabs manually:
 
     library tabs tabs.db -L 1  # open one tab
 
+Incremental surfing. 📈🏄 totally rad!
+
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.29.002)
+    xk media library subcommands (v1.29.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -302,15 +222,464 @@
     library listen music.tl.db -ct "House speakers"
 
 ### Hook into HackerNews
 
     wget https://github.com/chapmanjacobd/hn_mining/raw/main/hackernews_only_direct.tw.db
     library watch hackernews_only_direct.tw.db --random --ignore-errors
 
-## Watch/Listen Usage
+### Organize via separate databases.
+
+    library fsadd --audio both.db ./audiobooks/ ./podcasts/
+    library fsadd --audio audiobooks.db ./audiobooks/
+    library fsadd --audio podcasts.db ./podcasts/ ./another/more/secret/podcasts_folder/
+
+
+### Find large folders to curate
+
+<details><summary>lb bigdirs</summary>
+
+If you are looking for candidate folders for curation (ie. you need space but don't want to buy another hard drive).
+The bigdirs subcommand was written for that purpose:
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
+
+<details><summary>lb mv-list</summary>
+
+The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
+
+    $ lb fsadd --filesystem d.db ~/d/
+
+But this should definitely also work with xklb audio and video databases:
+
+    $ lb mv-list /mnt/d/ video.db
+
+The program will print a table with a sorted list of folders which are good candidates for moving. Candidates are determined by how many files are in the folder (so you don't spend hours waiting for folders with millions of tiny files to copy over). The default is 4 to 4000--but it can be adjusted via the --lower and --upper flags.
+
+    ...
+    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+    │ 4.0 GB   │       7 │ /mnt/d/71_Mealtime_Videos/unsorted/Miguel_4K/                                                                 │
+    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+    │ 5.7 GB   │      10 │ /mnt/d/71_Mealtime_Videos/unsorted/Bollywood_Premium/                                                         │
+    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
+    │ 2.3 GB   │       4 │ /mnt/d/71_Mealtime_Videos/chief_wiggum/                                                                       │
+    ╘══════════╧═════════╧═══════════════════════════════════════════════════════════════════════════════════════════════════════════════╛
+    6702 other folders not shown
+
+    ██╗███╗░░██╗░██████╗████████╗██████╗░██╗░░░██╗░█████╗░████████╗██╗░█████╗░███╗░░██╗░██████╗
+    ██║████╗░██║██╔════╝╚══██╔══╝██╔══██╗██║░░░██║██╔══██╗╚══██╔══╝██║██╔══██╗████╗░██║██╔════╝
+    ██║██╔██╗██║╚█████╗░░░░██║░░░██████╔╝██║░░░██║██║░░╚═╝░░░██║░░░██║██║░░██║██╔██╗██║╚█████╗░
+    ██║██║╚████║░╚═══██╗░░░██║░░░██╔══██╗██║░░░██║██║░░██╗░░░██║░░░██║██║░░██║██║╚████║░╚═══██╗
+    ██║██║░╚███║██████╔╝░░░██║░░░██║░░██║╚██████╔╝╚█████╔╝░░░██║░░░██║╚█████╔╝██║░╚███║██████╔╝
+    ╚═╝╚═╝░░╚══╝╚═════╝░░░░╚═╝░░░╚═╝░░╚═╝░╚═════╝░░╚════╝░░░░╚═╝░░░╚═╝░╚════╝░╚═╝░░╚══╝╚═════╝░
+
+    Type "done" when finished
+    Type "more" to see more files
+    Paste a folder (and press enter) to toggle selection
+    Type "*" to select all files in the most recently printed table
+
+Then it will give you a prompt:
+
+    Paste a path:
+
+Wherein you can copy and paste paths you want to move from the table and the program will keep track for you.
+
+    Paste a path: /mnt/d/75_MovieQueue/720p/s11/
+    26 selected paths: 162.1 GB ; future free space: 486.9 GB
+
+You can also press the up arrow or paste it again to remove it from the list:
+
+    Paste a path: /mnt/d/75_MovieQueue/720p/s11/
+    25 selected paths: 159.9 GB ; future free space: 484.7 GB
+
+After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
+
+    Paste a path: done
+
+        Folder list saved to /tmp/tmpa7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
+
+            rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmpa7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
+
+</details>
+
+
+### Scatter your data across disks with [mergerfs](https://github.com/trapexit/mergerfs)
+
+<details><summary>If you use mergerfs, you'll likely be interested in this</summary>
+
+    library scatter -h
+    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS database relative_paths ...
+
+    Balance size
+
+        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
+        Current path distribution:
+        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
+        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
+        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
+        │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d3 │            1 │ 717.6 kB     │ 717.6 kB      │ Jan 31         │ Jul 18 2022     │ yesterday      │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d4 │           82 │ 1.5 GB       │ 12.5 MB       │ Jan 31         │ Apr 22 2022     │ yesterday      │
+        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+
+        Simulated path distribution:
+        5845 files should be moved
+        20257 files should not be moved
+        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
+        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
+        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
+        │ /mnt/d1 │         9989 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d2 │        10185 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d3 │         1186 │ 53.6 GB      │ 30.8 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d4 │         1216 │ 49.5 GB      │ 29.5 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d5 │         1146 │ 53.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d6 │         1198 │ 48.8 GB      │ 30.6 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d7 │         1182 │ 52.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+        ### Move 1182 files to /mnt/d7 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpmr1628ij / /mnt/d7
+        ### Move 1198 files to /mnt/d6 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmp9yd75f6j / /mnt/d6
+        ### Move 1146 files to /mnt/d5 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
+        ### Move 1185 files to /mnt/d3 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
+        ### Move 1134 files to /mnt/d4 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
+
+    Balance device inodes for specific subfolder
+
+        $ library scatter -m /mnt/d1:/mnt/d2 ~/lb/fs/scatter.db subfolder --group count --sort 'size desc'
+
+    Scatter the most recent 100 files
+
+        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' ~/lb/fs/scatter.db /
+
+    Scatter without mountpoints (limited functionality; only good for balancing fs inodes)
+
+        $ library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
+
+
+    positional arguments:
+    database
+    relative_paths        Paths to scatter, relative to the root of your mergerfs mount; any path substring is valid
+
+    options:
+    -h, --help            show this help message and exit
+    --limit LIMIT, -L LIMIT, -l LIMIT, -queue LIMIT, --queue LIMIT
+    --policy POLICY, -p POLICY
+    --group GROUP, -g GROUP
+    --sort SORT, -s SORT  Sort files before moving
+    --usage, -u           Show disk usage
+    --verbose, -v
+    --srcmounts SRCMOUNTS, -m SRCMOUNTS
+                            /mnt/d1:/mnt/d2
+
+</details>
+
+### Pipe to [mnamer](https://github.com/jkwill87/mnamer)
+
+<details><summary>Rename poorly named files</summary>
+
+    pip install mnamer
+    mnamer --movie-directory ~/d/70_Now_Watching/ --episode-directory ~/d/70_Now_Watching/ \
+        --no-overwrite -b (library watch -p fd -s 'path : McCloud')
+    library fsadd ~/d/70_Now_Watching/
+
+</details>
+
+### Music alarm clock (via termux crontab)
+
+Wake up to your own music
+
+    30 7 * * * lb listen ./audio.db
+
+Wake up to your own music _only when you are *not* home_ (computer on local-only IP)
+
+    30 7 * * * timeout 0.4 nc -z 192.168.1.12 22 || lb listen --random
+
+Wake up to your own music on your Chromecast speaker group _only when you are home_
+
+    30 7 * * * ssh 192.168.1.12 lb listen --cast --cast-to "Bedroom pair"
+
+### Pipe to [lowcharts](https://github.com/juan-leon/lowcharts)
+
+<details><summary>$ lb watch -p f -col time_created | lowcharts timehist -w 80</summary>
+
+    Matches: 445183.
+    Each ∎ represents a count of 1896
+    [2022-04-13 03:16:05] [151689] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
+    [2022-04-19 07:59:37] [ 16093] ∎∎∎∎∎∎∎∎
+    [2022-04-25 12:43:09] [ 12019] ∎∎∎∎∎∎
+    [2022-05-01 17:26:41] [ 48817] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
+    [2022-05-07 22:10:14] [ 36259] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
+    [2022-05-14 02:53:46] [  3942] ∎∎
+    [2022-05-20 07:37:18] [  2371] ∎
+    [2022-05-26 12:20:50] [   517]
+    [2022-06-01 17:04:23] [  4845] ∎∎
+    [2022-06-07 21:47:55] [  2340] ∎
+    [2022-06-14 02:31:27] [   563]
+    [2022-06-20 07:14:59] [ 13836] ∎∎∎∎∎∎∎
+    [2022-06-26 11:58:32] [  1905] ∎
+    [2022-07-02 16:42:04] [  1269]
+    [2022-07-08 21:25:36] [  3062] ∎
+    [2022-07-15 02:09:08] [  9192] ∎∎∎∎
+    [2022-07-21 06:52:41] [ 11955] ∎∎∎∎∎∎
+    [2022-07-27 11:36:13] [ 50938] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
+    [2022-08-02 16:19:45] [ 70973] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
+    [2022-08-08 21:03:17] [  2598] ∎
+
+BTW, for some cols like time_deleted you'll need to specify a where clause so they aren't filtered out:
+
+    $ lb watch -p f -col time_deleted -w time_deleted'>'0 | lowcharts timehist -w 80
+
+![video width](https://user-images.githubusercontent.com/7908073/184737808-b96fbe65-a1d9-43c2-b6b4-4bdfab592190.png)
+
+![fps](https://user-images.githubusercontent.com/7908073/184738438-ee566a4b-2da0-4e6d-a4b3-9bfca036aa2a.png)
+
+</details>
+
+### Pipe to rsync
+
+<details><summary>Move files to your phone via syncthing</summary>
+
+I used to use rsync to move files because I want deletions to stick.
+I now use `lb relmv`. But this is still a good rsync example:
+
+    function mrmusic
+        rsync -a --remove-source-files --files-from=(
+            library lt ~/lb/audio.db -s /mnt/d/80_Now_Listening/ -p f \
+            --moved /mnt/d/80_Now_Listening/ /mnt/d/ | psub
+        ) /mnt/d/80_Now_Listening/ /mnt/d/
+
+        rsync -a --remove-source-files --files-from=(
+            library lt ~/lb/audio.db -w play_count=0 -u random -L 1200 -p f \
+            --moved /mnt/d/ /mnt/d/80_Now_Listening/ | psub
+        ) /mnt/d/ /mnt/d/80_Now_Listening/
+    end
+
+</details>
+
+### Backfill
+
+<details><summary>Backfill reddit databases with pushshift data</summary>
+
+[https://github.com/chapmanjacobd/reddit_mining/](https://github.com/chapmanjacobd/reddit_mining/)
+
+```fish
+for reddit_db in ~/lb/reddit/*.db
+    set subreddits (sqlite-utils $reddit_db 'select path from playlists' --tsv --no-headers | grep old.reddit.com | sed 's|https://old.reddit.com/r/\(.*\)/|\1|' | sed 's|https://old.reddit.com/user/\(.*\)/|u_\1|' | tr -d "\r")
+
+    ~/github/xk/reddit_mining/links/
+    for subreddit in $subreddits
+        if not test -e "$subreddit.csv"
+            echo "octosql -o csv \"select path,score,'https://old.reddit.com/r/$subreddit/' as playlist_path from `../reddit_links.parquet` where lower(playlist_path) = '$subreddit' order by score desc \" > $subreddit.csv"
+        end
+    end | parallel -j8
+
+    for subreddit in $subreddits
+        sqlite-utils upsert --pk path --alter --csv --detect-types $reddit_db media $subreddit.csv
+    end
+
+    library tubeadd --safe -i $reddit_db --playlist-db media
+end
+```
+
+</details>
+
+### Datasette
+
+Explore `library` databases in your browser
+
+    pip install datasette
+    datasette tv.db
+
+## Usage
+
+
+<details><summary>Add local media (fsadd)</summary>
+
+    $ library fsadd -h
+    usage: library fsadd [--audio | --video | --image |  --text | --filesystem] -c CATEGORY [database] paths ...
+
+    The default database type is video:
+        library fsadd tv.db ./tv/
+        library fsadd --video tv.db ./tv/  # equivalent
+
+    You can also create audio databases. Both audio and video use ffmpeg to read metadata:
+        library fsadd --audio audio.db ./music/
+
+    Image uses ExifTool:
+        library fsadd --image image.db ./photos/
+
+    Text will try to read files and save the contents into a searchable database:
+        library fsadd --text text.db ./documents_and_books/
+
+    Create a text database and scan with OCR and speech-recognition:
+        library fsadd --text --ocr --speech-recognition ocr.db ./receipts_and_messages/
+
+    Create a video database and read internal/external subtitle files into a searchable database:
+        library fsadd --scan-subtitles tv.search.db ./tv/ ./movies/
+
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
+    Normally only relevant filetypes are included. You can scan all files with this flag:
+        library fsadd --scan-all-files mixed.db ./tv-and-maybe-audio-only-files/
+        # I use that with this to keep my folders organized:
+        library watch -w 'video_count=0 and audio_count>=1' -pf mixed.db | parallel mv {} ~/d/82_Audiobooks/
+
+    Remove path roots with --force
+        library fsadd audio.db /mnt/d/Youtube/
+        [/mnt/d/Youtube] Path does not exist
+
+        library fsadd --force audio.db /mnt/d/Youtube/
+        [/mnt/d/Youtube] Path does not exist
+        [/mnt/d/Youtube] Building file list...
+        [/mnt/d/Youtube] Marking 28932 orphaned metadata records as deleted
+
+
+</details>
+
+<details><summary>Add online media (tubeadd)</summary>
+
+    $ library tubeadd -h
+    usage: library tubeadd [--audio | --video] [-c CATEGORY] [database] playlists ...
+
+    Create a dl database / add links to an existing database
+
+        library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
+
+    Add links from a line-delimited file
+
+        library tubeadd reddit.db --playlist-file ./my_yt_subscriptions.txt
+
+    Add metadata to links already in a database table
+
+        library tubeadd reddit.db --playlist-db media
+
+    You can also include a category for file organization
+
+        library tubeadd -c Mealtime dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
+
+    Files will be saved to <lb download prefix>/<lb tubeadd category>/
+
+        For example:
+        library tubeadd -c Cool ...
+        library download D:\'My Documents'\ ...
+        Media will be downloaded to 'D:\My Documents\Cool\'
+
+    Fetch extra metadata:
+
+        By default tubeadd will quickly add media at the expense of less metadata.
+        If you plan on using `library download` then it doesn't make sense to use `--extra`.
+        Downloading will add the extra metadata automatically to the database.
+        You can always fetch more metadata later via tubeupdate:
+        library tubeupdate tw.db --extra
+
+
+</details>
+
+<details><summary>Add reddit media (redditadd)</summary>
+
+    $ library redditadd -h
+    usage: library redditadd [--lookback N_DAYS] [--praw-site bot1] [database] paths ...
+
+    Fetch data for redditors and reddits:
+
+        library redditadd https://old.reddit.com/r/coolgithubprojects/ https://old.reddit.com/user/Diastro
+
+    If you have a file with a list of subreddits you can do this:
+
+        library redditadd --subreddits --db 96_Weird_History.db (cat ~/mc/96_Weird_History-reddit.txt)
+
+    Likewise for redditors:
+
+        library redditadd --redditors --db idk.db (cat ~/mc/shadow_banned.txt)
+
+
+</details>
+
+<details><summary>Create / Update a Hacker News database (hnadd)</summary>
+
+    $ library hnadd -h
+    usage: library hnadd [--oldest] database
+
+    Fetch latest stories first:
+
+        library hnadd hn.db -v
+        Fetching 154873 items (33212696 to 33367569)
+        Saving comment 33367568
+        Saving comment 33367543
+        Saving comment 33367564
+        ...
+
+    Fetch oldest stories first:
+
+        library hnadd --oldest hn.db
+
+
+</details>
+
+<details><summary>Add tabs (tabsadd)</summary>
+
+    $ library tabsadd -h
+    usage: library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--category CATEGORY] [--no-sanitize] DATABASE URLS ...
+
+    Adding one URL:
+
+        library tabsadd -f monthly -c travel ~/lb/tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
+
+        Depending on your shell you may need to escape the URL (add quotes)
+
+        If you use Fish shell know that you can enable features to make pasting easier:
+            set -U fish_features stderr-nocaret qmark-noglob regex-easyesc ampersand-nobg-in-token
+
+        Also I recommend turning Ctrl+Backspace into a super-backspace for repeating similar commands with long args:
+            echo 'bind \b backward-kill-bigword' >> ~/.config/fish/config.fish
+
+    Importing from a line-delimitated file:
+
+        library tabsadd -f yearly -c reddit ~/lb/tabs.db (cat ~/mc/yearly-subreddit.cron)
+
+
+
+</details>
+
+<details><summary>Watch / Listen</summary>
 
     $ library watch -h
     usage: library watch [database] [optional args]
 
     Control playback:
         To stop playback press Ctrl-C in either the terminal or mpv
 
@@ -561,298 +930,529 @@
         library watch --multiple-playback    # one per display; or two if only one display detected
         library watch --multiple-playback 4  # play four media at once, divide by available screens
         library watch -m 4 --screen-name eDP # play four media at once on specific screen
         library watch -m 4 --loop --crop     # play four cropped videos on a loop
         library watch -m 4 --hstack          # use hstack style
 
 
-## More examples
+</details>
 
-### Organize via separate databases.
+<details><summary>Search captions / subtitles</summary>
 
-    library fsadd --audio both.db ./audiobooks/ ./podcasts/
-    library fsadd --audio audiobooks.db ./audiobooks/
-    library fsadd --audio podcasts.db ./podcasts/ ./another/more/secret/podcasts_folder/
+    $ library search -h
+    usage: library search
 
+    Search text databases and subtitles
 
-### Find large folders to curate
+    $ library search fts.db boil
+        7 captions
+        /mnt/d/70_Now_Watching/DidubeTheLastStop-720p.mp4
+           33:46 I brought a real stainless steel boiler
+           33:59 The world is using only stainless boilers nowadays
+           34:02 The boiler is old and authentic
+           34:30 - This boiler? - Yes
+           34:44 I am not forcing you to buy this boiler…
+           34:52 Who will give her a one liter stainless steel boiler for one Lari?
+           34:54 Glass boilers cost two
 
-<details><summary>lb bigdirs</summary>
+    Search and open file
+    $ library search fts.db dashi --open
 
-Also, if you are just looking for folders which are candidates for curation (ie. I need space but don't want to buy a hard drive). The bigdirs subcommand was written for that purpose:
 
-    $ lb bigdirs fs/d.db
+</details>
 
-You may filter by folder depth (similar to QDirStat or WizTree)
+<details><summary>Open tabs</summary>
 
-    $ lb bigdirs --depth=3 audio.db
+    $ library tabs -h
+    usage: library tabs DATABASE
 
-There is also an flag to prioritize folders which have many files which have been deleted (for example you delete songs you don't like--now you can see who wrote those songs and delete all their other songs...)
+    Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
+
+        45 9 * * * DISPLAY=:0 library tabs /home/my/tabs.db
+
+    If things aren't working you can use `at` to simulate a similar environment as `cron`
+
+        echo 'fish -c "export DISPLAY=:0 && library tabs /full/path/to/tabs.db"' | at NOW
+
+    You can also invoke tabs manually:
+
+        library tabs -L 1  # open one tab
+
+    Print URLs
+
+        lb-dev tabs -w "frequency='yearly'" -p
+        ╒════════════════════════════════════════════════════════════════╤═════════════╤══════════════╕
+        │ path                                                           │ frequency   │ time_valid   │
+        ╞════════════════════════════════════════════════════════════════╪═════════════╪══════════════╡
+        │ https://old.reddit.com/r/Autonomia/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
+        ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/Cyberpunk/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
+        ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/ExperiencedDevs/top/?sort=top&t=year  │ yearly      │ Dec 31 1970  │
+
+        ...
+
+        ╘════════════════════════════════════════════════════════════════╧═════════════╧══════════════╛
+
+    View how many yearly tabs you have:
+
+        library tabs -w "frequency='yearly'" -p a
+        ╒═══════════╤═════════╕
+        │ path      │   count │
+        ╞═══════════╪═════════╡
+        │ Aggregate │     134 │
+        ╘═══════════╧═════════╛
+
+    Delete URLs
+
+        library tb -p -s cyber
+        ╒═══════════════════════════════════════╤═════════════╤══════════════╕
+        │ path                                  │ frequency   │ time_valid   │
+        ╞═══════════════════════════════════════╪═════════════╪══════════════╡
+        │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
+        │ p/?sort=top&t=year                    │             │              │
+        ├───────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
+        │ p/?sort=top&t=year                    │             │              │
+        ├───────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://www.reddit.com/r/cyberDeck/   │ yearly      │ Sep 05 2023  │
+        ╘═══════════════════════════════════════╧═════════════╧══════════════╛
+        library tb -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete
+        Removed 1 metadata records
+        library tb -p -s cyber
+        ╒═══════════════════════════════════════╤═════════════╤══════════════╕
+        │ path                                  │ frequency   │ time_valid   │
+        ╞═══════════════════════════════════════╪═════════════╪══════════════╡
+        │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
+        │ p/?sort=top&t=year                    │             │              │
+        ├───────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
+        │ p/?sort=top&t=year                    │             │              │
+        ╘═══════════════════════════════════════╧═════════════╧══════════════╛
 
-    $ lb bigdirs --sort-by deleted audio.db
 
 </details>
 
+<details><summary>Download media</summary>
 
-### Find candidates for freeing up space by moving to another mount point
+    $ library download -h
+    usage: library download database [--prefix /mnt/d/] --video | --audio
 
-<details><summary>lb mv-list</summary>
+    Download stuff in a random order.
 
-The program takes a mount point and a xklb database file. If you don't have a database file you can create one like this:
+        library download dl.db --prefix ~/output/path/root/
 
-    $ lb fsadd --filesystem d.db ~/d/
+    Download stuff in a random order, limited to the specified playlist URLs.
 
-But this should definitely also work with xklb audio and video databases:
+        library download dl.db https://www.youtube.com/c/BlenderFoundation/videos
 
-    $ lb mv-list /mnt/d/ video.db
+    Files will be saved to <lb download prefix>/<lb download category>/
 
-The program will print a table with a sorted list of folders which are good candidates for moving. Candidates are determined by how many files are in the folder (so you don't spend hours waiting for folders with millions of tiny files to copy over). The default is 4 to 4000--but it can be adjusted via the --lower and --upper flags.
+        For example:
+        library dladd Cool ...
+        library download D:\'My Documents'\ ...
+        Media will be downloaded to 'D:\My Documents\Cool\'
 
-    ...
-    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-    │ 4.0 GB   │       7 │ /mnt/d/71_Mealtime_Videos/unsorted/Miguel_4K/                                                                 │
-    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-    │ 5.7 GB   │      10 │ /mnt/d/71_Mealtime_Videos/unsorted/Bollywood_Premium/                                                         │
-    ├──────────┼─────────┼───────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
-    │ 2.3 GB   │       4 │ /mnt/d/71_Mealtime_Videos/chief_wiggum/                                                                       │
-    ╘══════════╧═════════╧═══════════════════════════════════════════════════════════════════════════════════════════════════════════════╛
-    6702 other folders not shown
+    Print list of queued up downloads
 
-    ██╗███╗░░██╗░██████╗████████╗██████╗░██╗░░░██╗░█████╗░████████╗██╗░█████╗░███╗░░██╗░██████╗
-    ██║████╗░██║██╔════╝╚══██╔══╝██╔══██╗██║░░░██║██╔══██╗╚══██╔══╝██║██╔══██╗████╗░██║██╔════╝
-    ██║██╔██╗██║╚█████╗░░░░██║░░░██████╔╝██║░░░██║██║░░╚═╝░░░██║░░░██║██║░░██║██╔██╗██║╚█████╗░
-    ██║██║╚████║░╚═══██╗░░░██║░░░██╔══██╗██║░░░██║██║░░██╗░░░██║░░░██║██║░░██║██║╚████║░╚═══██╗
-    ██║██║░╚███║██████╔╝░░░██║░░░██║░░██║╚██████╔╝╚█████╔╝░░░██║░░░██║╚█████╔╝██║░╚███║██████╔╝
-    ╚═╝╚═╝░░╚══╝╚═════╝░░░░╚═╝░░░╚═╝░░╚═╝░╚═════╝░░╚════╝░░░░╚═╝░░░╚═╝░╚════╝░╚═╝░░╚══╝╚═════╝░
+        library download --print
 
-    Type "done" when finished
-    Type "more" to see more files
-    Paste a folder (and press enter) to toggle selection
-    Type "*" to select all files in the most recently printed table
+    Print list of saved playlists
 
-Then it will give you a prompt:
+        library playlists dl.db -p a
 
-    Paste a path:
+    Print download queue groups
 
-Wherein you can copy and paste paths you want to move from the table and the program will keep track for you.
+        library dlstatus audio.db
+        ╒═════════════════════╤════════════╤══════════════════╤════════════════════╤══════════╕
+        │ category            │ ie_key     │ duration         │   never_downloaded │   errors │
+        ╞═════════════════════╪════════════╪══════════════════╪════════════════════╪══════════╡
+        │ 81_New_Music        │ Soundcloud │                  │                 10 │        0 │
+        ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
+        │ 81_New_Music        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
+        │                     │            │ and 20 minutes   │                    │          │
+        ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Playlist-less media │ Youtube    │ 7.68 minutes     │                 99 │        1 │
+        ╘═════════════════════╧════════════╧══════════════════╧════════════════════╧══════════╛
 
-    Paste a path: /mnt/d/75_MovieQueue/720p/s11/
-    26 selected paths: 162.1 GB ; future free space: 486.9 GB
 
-You can also press the up arrow or paste it again to remove it from the list:
+</details>
 
-    Paste a path: /mnt/d/75_MovieQueue/720p/s11/
-    25 selected paths: 159.9 GB ; future free space: 484.7 GB
+<details><summary>Show Download Status (dlstatus)</summary>
 
-After you are done selecting folders you can press ctrl-d and it will save the list to a tmp file:
+    $ library dlstatus -h
+    usage: library dlstatus [database]
 
-    Paste a path: done
+    Print download queue groups
 
-        Folder list saved to /tmp/tmpa7x_75l8. You may want to use the following command to move files to an EMPTY folder target:
+        library dlstatus video.db
+        ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
+        │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
+        ╞═════════════════════╪═════════════╪══════════════════╪════════════════════╪══════════╡
+        │ 71_Mealtime_Videos  │ Youtube     │ 3 hours and 2.07 │                 76 │        0 │
+        │                     │             │ minutes          │                    │          │
+        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ 75_MovieQueue       │ Dailymotion │                  │                 53 │        0 │
+        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ 75_MovieQueue       │ Youtube     │ 1 day, 18 hours  │                 30 │        0 │
+        │                     │             │ and 6 minutes    │                    │          │
+        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Dailymotion         │ Dailymotion │                  │                186 │      198 │
+        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Uncategorized       │ Youtube     │ 1 hour and 52.18 │                  1 │        0 │
+        │                     │             │ minutes          │                    │          │
+        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Vimeo               │ Vimeo       │                  │                253 │       49 │
+        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube             │ Youtube     │ 2 years, 4       │              51676 │      197 │
+        │                     │             │ months, 15 days  │                    │          │
+        │                     │             │ and 6 hours      │                    │          │
+        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Playlist-less media │ Youtube     │ 4 months, 23     │               2686 │        7 │
+        │                     │             │ days, 19 hours   │                    │          │
+        │                     │             │ and 33 minutes   │                    │          │
+        ╘═════════════════════╧═════════════╧══════════════════╧════════════════════╧══════════╛
+
+    Simulate --safe flag
+
+        library dlstatus video.db --safe
+
+    Show only download attempts with errors
+
+        library dlstatus video.db --errors
 
-            rsync -a --info=progress2 --no-inc-recursive --remove-source-files --files-from=/tmp/tmpa7x_75l8 -r --relative -vv --dry-run / jim:/free/real/estate/
 
 </details>
 
+<details><summary>Update local media (fsupdate)</summary>
 
-### Scatter your data across disks with [mergerfs](https://github.com/trapexit/mergerfs)
+    $ library fsupdate -h
+    usage: library fsupdate database
 
-<details><summary>If you use mergerfs, you'll likely be interested in this</summary>
+    Update each path previously saved:
 
-    library scatter -h
-    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS database relative_paths ...
+        library fsupdate database
 
-    Balance size
 
-        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
-        Current path distribution:
-        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
-        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
-        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
-        │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d3 │            1 │ 717.6 kB     │ 717.6 kB      │ Jan 31         │ Jul 18 2022     │ yesterday      │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d4 │           82 │ 1.5 GB       │ 12.5 MB       │ Jan 31         │ Apr 22 2022     │ yesterday      │
-        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+</details>
 
-        Simulated path distribution:
-        5845 files should be moved
-        20257 files should not be moved
-        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
-        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
-        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
-        │ /mnt/d1 │         9989 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d2 │        10185 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d3 │         1186 │ 53.6 GB      │ 30.8 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d4 │         1216 │ 49.5 GB      │ 29.5 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d5 │         1146 │ 53.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d6 │         1198 │ 48.8 GB      │ 30.6 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
-        │ /mnt/d7 │         1182 │ 52.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
-        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
-        ### Move 1182 files to /mnt/d7 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpmr1628ij / /mnt/d7
-        ### Move 1198 files to /mnt/d6 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmp9yd75f6j / /mnt/d6
-        ### Move 1146 files to /mnt/d5 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
-        ### Move 1185 files to /mnt/d3 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
-        ### Move 1134 files to /mnt/d4 with this command: ###
-        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
+<details><summary>Update online media (tubeupdate)</summary>
 
-    Balance device inodes for specific subfolder
+    $ library tubeupdate -h
+    usage: library tubeupdate [--audio | --video] [-c CATEGORY] [database]
 
-        $ library scatter -m /mnt/d1:/mnt/d2 ~/lb/fs/scatter.db subfolder --group count --sort 'size desc'
+    Fetch the latest videos for every playlist saved in your database
 
-    Scatter the most recent 100 files
+        library tubeupdate educational.db
 
-        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' ~/lb/fs/scatter.db /
+    Or limit to specific categories...
 
-    Scatter without mountpoints (limited functionality; only good for balancing fs inodes)
+        library tubeupdate -c "Bob Ross" educational.db
 
-        $ library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
+    Run with --optimize to add indexes (might speed up searching but the size will increase):
 
+        library tubeupdate --optimize examples/music.tl.db
 
-    positional arguments:
-    database
-    relative_paths        Paths to scatter, relative to the root of your mergerfs mount; any path substring is valid
+    Fetch extra metadata:
+
+        By default tubeupdate will quickly add media.
+        You can run with --extra to fetch more details: (best resolution width, height, subtitle tags, etc)
+
+        library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
 
-    options:
-    -h, --help            show this help message and exit
-    --limit LIMIT, -L LIMIT, -l LIMIT, -queue LIMIT, --queue LIMIT
-    --policy POLICY, -p POLICY
-    --group GROUP, -g GROUP
-    --sort SORT, -s SORT  Sort files before moving
-    --usage, -u           Show disk usage
-    --verbose, -v
-    --srcmounts SRCMOUNTS, -m SRCMOUNTS
-                            /mnt/d1:/mnt/d2
 
 </details>
 
-### Pipe to [mnamer](https://github.com/jkwill87/mnamer)
+<details><summary>Update reddit media (redditupdate)</summary>
 
-<details><summary>Rename poorly named files</summary>
+    $ library redditupdate -h
+    usage: library redditupdate [--audio | --video] [-c CATEGORY] [--lookback N_DAYS] [--praw-site bot1] [database]
+
+    Fetch the latest posts for every subreddit/redditor saved in your database
+
+        library redditupdate edu_subreddits.db
 
-    pip install mnamer
-    mnamer --movie-directory ~/d/70_Now_Watching/ --episode-directory ~/d/70_Now_Watching/ \
-        --no-overwrite -b (library watch -p fd -s 'path : McCloud')
-    library fsadd ~/d/70_Now_Watching/
 
 </details>
 
-### Music alarm clock (via termux crontab)
+<details><summary>Convert pushshift data to reddit.db format</summary>
 
-Wake up to your own music
+    $ library pushshift -h
+    usage: library pushshift [database] < stdin
 
-    30 7 * * * lb listen ./audio.db
+    Download data (about 600GB jsonl.zst; 6TB uncompressed)
 
-Wake up to your own music _only when you are *not* home_ (computer on local-only IP)
+        wget -e robots=off -r -k -A zst https://files.pushshift.io/reddit/submissions/
 
-    30 7 * * * timeout 0.4 nc -z 192.168.1.12 22 || lb listen --random
+    Load data from files via unzstd
 
-Wake up to your own music on your Chromecast speaker group _only when you are home_
+        unzstd --memory=2048MB --stdout RS_2005-07.zst | library pushshift pushshift.db
 
-    30 7 * * * ssh 192.168.1.12 lb listen --cast --cast-to "Bedroom pair"
+    Or multiple (output is about 1.5TB SQLITE fts-searchable):
 
-### Pipe to [lowcharts](https://github.com/juan-leon/lowcharts)
+        for f in psaw/files.pushshift.io/reddit/submissions/*.zst
+            echo "unzstd --memory=2048MB --stdout $f | library pushshift (basename $f).db"
+            library optimize (basename $f).db
+        end | parallel -j5
 
-<details><summary>$ lb watch -p f -col time_created | lowcharts timehist -w 80</summary>
 
-    Matches: 445183.
-    Each ∎ represents a count of 1896
-    [2022-04-13 03:16:05] [151689] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
-    [2022-04-19 07:59:37] [ 16093] ∎∎∎∎∎∎∎∎
-    [2022-04-25 12:43:09] [ 12019] ∎∎∎∎∎∎
-    [2022-05-01 17:26:41] [ 48817] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
-    [2022-05-07 22:10:14] [ 36259] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
-    [2022-05-14 02:53:46] [  3942] ∎∎
-    [2022-05-20 07:37:18] [  2371] ∎
-    [2022-05-26 12:20:50] [   517]
-    [2022-06-01 17:04:23] [  4845] ∎∎
-    [2022-06-07 21:47:55] [  2340] ∎
-    [2022-06-14 02:31:27] [   563]
-    [2022-06-20 07:14:59] [ 13836] ∎∎∎∎∎∎∎
-    [2022-06-26 11:58:32] [  1905] ∎
-    [2022-07-02 16:42:04] [  1269]
-    [2022-07-08 21:25:36] [  3062] ∎
-    [2022-07-15 02:09:08] [  9192] ∎∎∎∎
-    [2022-07-21 06:52:41] [ 11955] ∎∎∎∎∎∎
-    [2022-07-27 11:36:13] [ 50938] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
-    [2022-08-02 16:19:45] [ 70973] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
-    [2022-08-08 21:03:17] [  2598] ∎
+</details>
 
-BTW, for some cols like time_deleted you'll need to specify a where clause so they aren't filtered out:
+<details><summary>List playlists</summary>
 
-    $ lb watch -p f -col time_deleted -w time_deleted'>'0 | lowcharts timehist -w 80
+    $ library playlists -h
+    usage: library playlists [database] [--aggregate] [--fields] [--json] [--delete ...]
+
+    List of Playlists
+
+        library playlists
+        ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╕
+        │ ie_key   │ title              │ path                                                                     │
+        ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╡
+        │ Youtube  │ Highlights of Life │ https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n │
+        ╘══════════╧════════════════════╧══════════════════════════════════════════════════════════════════════════╛
+
+    Aggregate Report of Videos in each Playlist
+
+        library playlists -p a
+        ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╤═══════════════╤═════════╕
+        │ ie_key   │ title              │ path                                                                     │ duration      │   count │
+        ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╪═══════════════╪═════════╡
+        │ Youtube  │ Highlights of Life │ https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n │ 53.28 minutes │      15 │
+        ╘══════════╧════════════════════╧══════════════════════════════════════════════════════════════════════════╧═══════════════╧═════════╛
+        1 playlist
+        Total duration: 53.28 minutes
+
+    Print only playlist urls:
+        Useful for piping to other utilities like xargs or GNU Parallel.
+        library playlists -p f
+        https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n
+
+    Remove a playlist/channel and all linked videos:
+        library playlists --remove https://vimeo.com/canal180
 
-![video width](https://user-images.githubusercontent.com/7908073/184737808-b96fbe65-a1d9-43c2-b6b4-4bdfab592190.png)
 
-![fps](https://user-images.githubusercontent.com/7908073/184738438-ee566a4b-2da0-4e6d-a4b3-9bfca036aa2a.png)
 
 </details>
 
-### Pipe to rsync
+<details><summary>Blocklist a channel</summary>
 
-<details><summary>Move files to your phone via syncthing</summary>
+    $ library block -h
+    usage: library block database [playlists ...]
 
-I used to use rsync to move files because I want deletions to stick.
-I now use `lb relmv`. But this is still a good rsync example:
+    Blocklist specific URLs (eg. YouTube channels, etc). With YT URLs this will block
+    videos from the playlist uploader
 
-    function mrmusic
-        rsync -a --remove-source-files --files-from=(
-            library lt ~/lb/audio.db -s /mnt/d/80_Now_Listening/ -p f \
-            --moved /mnt/d/80_Now_Listening/ /mnt/d/ | psub
-        ) /mnt/d/80_Now_Listening/ /mnt/d/
+        library block dl.db https://annoyingwebsite/etc/
+
+    Use with the all-deleted-playlists flag to delete any previously downloaded files from the playlist uploader
+
+        library block dl.db --all-deleted-playlists https://annoyingwebsite/etc/
 
-        rsync -a --remove-source-files --files-from=(
-            library lt ~/lb/audio.db -w play_count=0 -u random -L 1200 -p f \
-            --moved /mnt/d/ /mnt/d/80_Now_Listening/ | psub
-        ) /mnt/d/ /mnt/d/80_Now_Listening/
-    end
 
 </details>
 
-### Backfill
+<details><summary>Show large folders (bigdirs)</summary>
 
-<details><summary>Backfill reddit databases with pushshift data</summary>
+    $ library bigdirs -h
+    usage: library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by "deleted" | "played"] [--size=+5MB]
 
-[https://github.com/chapmanjacobd/reddit_mining/](https://github.com/chapmanjacobd/reddit_mining/)
+    See what folders take up space
 
-```fish
-for reddit_db in ~/lb/reddit/*.db
-    set subreddits (sqlite-utils $reddit_db 'select path from playlists' --tsv --no-headers | grep old.reddit.com | sed 's|https://old.reddit.com/r/\(.*\)/|\1|' | sed 's|https://old.reddit.com/user/\(.*\)/|u_\1|' | tr -d "\r")
+        lb bigdirs video.db
+        lb bigdirs audio.db
+        lb bigdirs fs.db
 
-    ~/github/xk/reddit_mining/links/
-    for subreddit in $subreddits
-        if not test -e "$subreddit.csv"
-            echo "octosql -o csv \"select path,score,'https://old.reddit.com/r/$subreddit/' as playlist_path from `../reddit_links.parquet` where lower(playlist_path) = '$subreddit' order by score desc \" > $subreddit.csv"
-        end
-    end | parallel -j8
 
-    for subreddit in $subreddits
-        sqlite-utils upsert --pk path --alter --csv --detect-types $reddit_db media $subreddit.csv
-    end
+</details>
+
+<details><summary>Copy play history (copy-play-counts)</summary>
+
+    $ library copy-play-counts -h
+    usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
+
+    Copy play count information between databases
+
+        lb copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 
-    library tubeadd --safe -i $reddit_db --playlist-db media
-end
-```
 
 </details>
 
-### Datasette
+<details><summary>Dedupe music</summary>
 
-Explore `library` databases in your browser
+    $ library dedupe -h
+    usage: library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
 
-    pip install datasette
-    datasette tv.db
+    Dedupe your files
+
+
+</details>
+
+<details><summary>Re-optimize database</summary>
+
+    $ library optimize -h
+    usage: library optimize DATABASE [--force]
+
+    Optimize library databases
+
+    The force flag is usually unnecessary and it can take much longer
+
+
+</details>
+
+<details><summary>Re-download media (redownload)</summary>
+
+    $ library redownload -h
+    usage: library redownload DATABASE
+
+    If you have previously downloaded YouTube or other online media, but your
+    hard drive failed or you accidentally deleted something, and if that media
+    is still accessible from the same URL, this script can help to redownload
+    everything that was scanned-as-deleted between two timestamps.
+
+    List deletions:
+
+        $ library redownload news.db
+        Deletions:
+        ╒═════════════════════╤═════════╕
+        │ time_deleted        │   count │
+        ╞═════════════════════╪═════════╡
+        │ 2023-01-26T00:31:26 │     120 │
+        ├─────────────────────┼─────────┤
+        │ 2023-01-26T19:54:42 │      18 │
+        ├─────────────────────┼─────────┤
+        │ 2023-01-26T20:45:24 │      26 │
+        ╘═════════════════════╧═════════╛
+        Showing most recent 3 deletions. Use -l to change this limit
+
+    Mark videos as candidates for download via specific deletion timestamp:
+
+        $ library redownload city.db 2023-01-26T19:54:42
+        ╒══════════╤════════════════╤═════════════════╤═══════════════════╤═════════╤══════════╤═══════╤══════════════════╤════════════════════════════════════════════════════════════════════════════════════════════════════════╕
+        │ size     │ time_created   │ time_modified   │ time_downloaded   │   width │   height │   fps │ duration         │ path                                                                                                   │
+        ╞══════════╪════════════════╪═════════════════╪═══════════════════╪═════════╪══════════╪═══════╪══════════════════╪════════════════════════════════════════════════════════════════════════════════════════════════════════╡
+        │ 697.7 MB │ Apr 13 2022    │ Mar 11 2022     │ Oct 19            │    1920 │     1080 │    30 │ 21.22 minutes    │ /mnt/d/76_CityVideos/PRAIA DE BARRA DE JANGADA CANDEIAS JABOATÃO                                       │
+        │          │                │                 │                   │         │          │       │                  │ RECIFE PE BRASIL AVENIDA BERNARDO VIEIRA DE MELO-4Lx3hheMPmg.mp4
+        ...
+
+    ...or between two timestamps inclusive:
+
+        $ library redownload city.db 2023-01-26T19:54:42 2023-01-26T20:45:24
+
+
+</details>
+
+<details><summary>Merge online and local data (merge-online-local)</summary>
+
+    $ library merge-online-local -h
+    usage: library merge-online-local DATABASE
+
+    If you have previously downloaded YouTube or other online media, you can dedupe
+    your database and combine the online and local media records as long as your
+    files have the youtube-dl / yt-dlp id in the filename.
+
+
+</details>
+
+<details><summary>Convert selftext links to media table (reddit-selftext)</summary>
+
+    $ library reddit-selftext -h
+    usage: library reddit-selftext DATABASE
+
+    Extract URLs from reddit selftext from the reddit_posts table to the media table
+
+
+</details>
+
+<details><summary>Merge SQLITE databases (merge-dbs)</summary>
+
+    $ library merge-dbs -h
+    usage: library merge-dbs DEST_DB SOURCE_DB ... [--upsert pk1[,pk2]]
+
+    Merge database data and tables
+
+        lb merge-dbs --upsert --pk path video.db tv.db movies.db
+        lb merge-dbs --table media,playlists --pk path audio.db music.db podcasts.db
+
+
+</details>
+
+<details><summary>Sort lines by similarity (cluster-sort)</summary>
+
+    $ library cluster-sort -h
+    usage: library cluster-sort [input_path | stdin] [output_path | stdout]
+
+    Group lines of text into sorted output
+
+
+</details>
+
+<details><summary>Move files preserving parent folder hierarchy (relmv)</summary>
+
+    $ library relmv -h
+    usage: library relmv [--dry-run] SOURCE ... DEST
+
+    Move files/folders without losing hierarchy metadata
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
+
+
+</details>
+
+<details><summary>Automatic tab loader (surf)</summary>
+
+    $ library surf -h
+    usage: library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
+
+    Streaming tab loader: press ctrl+c to stop.
+
+    Open tabs from a line-delimited file:
+
+        cat tabs.txt | library surf -n 5
+
+    You will likely want to use this setting in `about:config`
+
+        browser.tabs.loadDivertedInBackground = True
+
+    If you prefer GUI, check out https://unli.xyz/tabsender/
+
+
+</details>
+
+<details><summary>Clean filenames (christen)</summary>
+
+    $ library christen -h
+    usage: library christen DATABASE [--run]
+
+    Rename files to be somewhat normalized
+
+    Default mode is dry-run
+
+        lb christen fs.db
+
+    To actually do stuff use the run flag
+
+        lb christen audio.db --run
+
+    You can optionally replace all the spaces in your filenames with dots
+
+        lb christen --dot-space video.db
+
+
+</details>
+
+
+You can expand all by running this in your browser console:
+
+```js
+(() => { const readmeDiv = document.getElementById("readme"); const detailsElements = readmeDiv.getElementsByTagName("details"); for (let i = 0; i < detailsElements.length; i++) { detailsElements[i].setAttribute("open", "true"); } })();
+```
```


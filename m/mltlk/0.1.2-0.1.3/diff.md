# Comparing `tmp/mltlk-0.1.2.tar.gz` & `tmp/mltlk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltlk-0.1.2.tar", last modified: Fri May 26 09:50:42 2023, max compression
+gzip compressed data, was "dist/mltlk-0.1.3.tar", last modified: Mon May 29 08:26:33 2023, max compression
```

## Comparing `mltlk-0.1.2.tar` & `mltlk-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 09:50:42.745453 mltlk-0.1.2/
--rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.2/.gitignore
--rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.2/LICENSE
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-26 09:50:42.744697 mltlk-0.1.2/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.2/README.md
--rw-r--r--   0 johanhagelback   (503) staff       (20)    31370 2023-05-26 09:49:14.000000 mltlk-0.1.2/Spiral.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-26 09:48:44.000000 mltlk-0.1.2/Weather.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    50437 2023-05-26 09:49:20.000000 mltlk-0.1.2/Wikipedia.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    49851 2023-05-26 09:44:45.000000 mltlk-0.1.2/Wikipedia_word2vec.ipynb
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 09:50:42.718924 mltlk-0.1.2/data/
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.2/data/spiral.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.2/data/weather.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.2/data/wikipedia_300.csv.gz
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 09:50:42.733923 mltlk-0.1.2/mltlk/
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)       73 2023-05-26 08:58:43.000000 mltlk-0.1.2/mltlk/__init__.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)    32015 2023-05-26 09:48:27.000000 mltlk-0.1.2/mltlk/ml.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.2/mltlk/resampling.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)      337 2023-05-25 12:06:32.000000 mltlk-0.1.2/mltlk/utils.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4978 2023-05-26 07:38:19.000000 mltlk-0.1.2/mltlk/word2vec.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-26 09:50:42.743215 mltlk-0.1.2/mltlk.egg-info/
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-26 09:50:42.000000 mltlk-0.1.2/mltlk.egg-info/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      391 2023-05-26 09:50:42.000000 mltlk-0.1.2/mltlk.egg-info/SOURCES.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-26 09:50:42.000000 mltlk-0.1.2/mltlk.egg-info/dependency_links.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-26 09:50:42.000000 mltlk-0.1.2/mltlk.egg-info/requires.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-26 09:50:42.000000 mltlk-0.1.2/mltlk.egg-info/top_level.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-26 09:50:42.745715 mltlk-0.1.2/setup.cfg
--rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-26 08:58:35.000000 mltlk-0.1.2/setup.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-29 08:26:33.419133 mltlk-0.1.3/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.3/.gitignore
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.3/LICENSE
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-29 08:26:33.418026 mltlk-0.1.3/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.3/README.md
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    31369 2023-05-26 11:59:23.000000 mltlk-0.1.3/Spiral.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-26 11:58:57.000000 mltlk-0.1.3/Weather.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    50617 2023-05-29 08:24:46.000000 mltlk-0.1.3/Wikipedia.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    49905 2023-05-29 08:25:32.000000 mltlk-0.1.3/Wikipedia_word2vec.ipynb
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-29 08:26:33.397067 mltlk-0.1.3/data/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.3/data/spiral.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.3/data/weather.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.3/data/wikipedia_300.csv.gz
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-29 08:26:33.410925 mltlk-0.1.3/mltlk/
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)       73 2023-05-26 11:47:03.000000 mltlk-0.1.3/mltlk/__init__.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    32049 2023-05-29 08:23:55.000000 mltlk-0.1.3/mltlk/ml.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.3/mltlk/resampling.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-29 06:55:45.000000 mltlk-0.1.3/mltlk/utils.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.3/mltlk/word2vec.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-29 08:26:33.416013 mltlk-0.1.3/mltlk.egg-info/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-29 08:26:32.000000 mltlk-0.1.3/mltlk.egg-info/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      412 2023-05-29 08:26:33.000000 mltlk-0.1.3/mltlk.egg-info/SOURCES.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-29 08:26:32.000000 mltlk-0.1.3/mltlk.egg-info/dependency_links.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-29 08:26:33.000000 mltlk-0.1.3/mltlk.egg-info/requires.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-29 08:26:33.000000 mltlk-0.1.3/mltlk.egg-info/top_level.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-29 08:26:33.419375 mltlk-0.1.3/setup.cfg
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-26 11:47:12.000000 mltlk-0.1.3/setup.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-29 08:26:33.416995 mltlk-0.1.3/stopwords/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.3/stopwords/custom.csv
```

### Comparing `mltlk-0.1.2/LICENSE` & `mltlk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.2/Spiral.ipynb` & `mltlk-0.1.3/Spiral.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996851851851851%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.3\\n']}}}, 8: {'outputs': {0: {'text': {insert: "*

 * *            "[(0, 'Building and evaluating model using 10-fold cross validaton took "*

 * *            "\\x1b[34m6.90\\x1b[0m sec\\n')], delete: [0]}}}}, 10: {'outputs': {0: {'text': "*

 * *            "{insert: [(0, 'Building and evaluating model using 10-fold cross validaton took "*

 * *            "\\x1b[34m1.12\\x1b[0m sec\\n')], delete: [0]}}}}, 12: {'outputs': {0: {'text': "*

 * *            "['\\x1b[1m\\x1b[33mInfo: \\x1b[0 […]*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.2\n"
+                        "0.1.3\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -102,15 +102,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m14.39\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m6.90\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>97.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.36%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>97.33%</td></tr></table>"
@@ -169,15 +169,15 @@
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.88\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.12\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>97.68%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.76%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>97.67%</td></tr></table>"
@@ -237,15 +237,15 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.20\u001b[0m sec\n"
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.12\u001b[0m sec\n"
                     ]
                 }
             ],
             "source": [
                 "build_model(RandomForestClassifier(), session)"
             ]
         },
```

### Comparing `mltlk-0.1.2/Weather.ipynb` & `mltlk-0.1.3/Weather.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996362433862434%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.3\\n']}}}, 7: {'outputs': {0: {'text': {insert: "*

 * *            "[(0, 'Building and evaluating model using 10-fold cross validaton took "*

 * *            "\\x1b[34m1.01\\x1b[0m sec\\n')], delete: [0]}}}}, 9: {'outputs': {0: {'text': "*

 * *            "['\\x1b[1m\\x1b[33mInfo: \\x1b[0mBuilding final model on all data took "*

 * *            "\\x1b[34m0.18\\x1b[0m sec\\n']}}}}"}*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.2\n"
+                        "0.1.3\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -96,15 +96,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.07\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.01\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>64.29%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>63.24%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>62.86%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>64.29%</td></tr></table>"
@@ -182,15 +182,15 @@
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.12\u001b[0m sec\n"
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.18\u001b[0m sec\n"
                     ]
                 }
             ],
             "source": [
                 "build_model(RandomForestClassifier(), session)"
             ]
         },
```

### Comparing `mltlk-0.1.2/Wikipedia.ipynb` & `mltlk-0.1.3/Wikipedia.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992832341269842%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.3\\n']}}}, 3: {'outputs': {0: {'text': {insert: "*

 * *            "[(1, '\\x1b[1m\\x1b[33mInfo: \\x1b[0mLoad 180 stopwords from \\x1b[36menglish, "*

 * *            "stopwords/custom.csv\\x1b[0m\\n'), (2, '\\x1b[1m\\x1b[33mInfo: \\x1b[0mUsed "*

 * *            "bag-of-words with stopwords removed and TF-IDF\\n')], delete: [2, 1]}}}, 'source': "*

 * *            '{insert: [(3, \'    "stopwords": ["english", "stopwords/custom.csv"],\\n\')], delete: '*

 * *            '[3]}}, 5: {\'outp […]*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.2\n"
+                        "0.1.3\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -42,25 +42,25 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u001b[1m\u001b[33mInfo: \u001b[0mClean texts keeping letters and digits\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mUsed bag-of-words with stopwords \u001b[36menglish\u001b[0m removed\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mUsed TF-IDF\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mLoad 180 stopwords from \u001b[36menglish, stopwords/custom.csv\u001b[0m\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mUsed bag-of-words with stopwords removed and TF-IDF\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mLoaded \u001b[34m300\u001b[0m examples in \u001b[34m2\u001b[0m categories\n"
                     ]
                 }
             ],
             "source": [
                 "session = load_data(\"data/wikipedia_300.csv.gz\", conf={\n",
                 "    \"preprocess\": \"bag-of-words\",\n",
                 "    \"TF-IDF\": True,\n",
-                "    \"stopwords\": \"english\",\n",
+                "    \"stopwords\": [\"english\", \"stopwords/custom.csv\"],\n",
                 "    \"clean_text\": \"letters digits\",\n",
                 "})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -72,15 +72,15 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>150</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>150</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>100.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Examples:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>300</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Features:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>53124</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Categories:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>2</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>150</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>150</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>50.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>100.0%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Examples:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>300</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Features:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>53123</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Categories:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>2</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -103,15 +103,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.33\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.31\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.37%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>95.33%</td></tr></table>"
@@ -210,15 +210,15 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.34\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.32\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.37%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>95.33%</td></tr></table>"
@@ -278,15 +278,15 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.04\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.04\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mExample is predicted as \u001b[32mGames\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "build_model(LinearSVC(), session)\n",
                 "predict(\"This is an article about gamers - people who love playing games\", session)"
@@ -305,15 +305,15 @@
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mSession saved to \u001b[34msessions/wikipedia.gz\u001b[0m\n"
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mSession saved to \u001b[36msessions/wikipedia.gz\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "save_session(session, \"wikipedia\")    "
             ]
         },
@@ -329,15 +329,15 @@
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mSession loaded from \u001b[34msessions/wikipedia.gz\u001b[0m\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mSession loaded from \u001b[36msessions/wikipedia.gz\u001b[0m (created at \u001b[34m2023-05-29 10:24:37\u001b[0m from file \u001b[36mdata/wikipedia_300.csv.gz\u001b[0m)\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mExample is predicted as \u001b[32mGames\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "loaded_session = load_session(\"wikipedia\")\n",
                 "predict(\"This is an article about gamers - people who love playing games\", loaded_session)"
```

### Comparing `mltlk-0.1.2/Wikipedia_word2vec.ipynb` & `mltlk-0.1.3/Wikipedia_word2vec.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962106717687075%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.3\\n']}}}, 3: {'outputs': {0: {'text': {insert: "*

 * *            "[(1, '\\x1b[1m\\x1b[33mInfo: \\x1b[0mLoad 180 stopwords from \\x1b[36menglish, "*

 * *            "stopwords/custom.csv\\x1b[0m\\n'), (2, '\\x1b[1m\\x1b[33mInfo: \\x1b[0mWord2vec model "*

 * *            "generated in \\x1b[34m5.32\\x1b[0m sec\\n'), (4, '\\x1b[1m\\x1b[33mInfo: "*

 * *            "\\x1b[0mWord2vec embeddings generated in \\x1b[34m13.96\\x1b[0m sec\\n')], delete: "*

 * *            '[4, 2, 1]}}}, \'sour […]*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.2\n"
+                        "0.1.3\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -42,28 +42,28 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u001b[1m\u001b[33mInfo: \u001b[0mClean texts keeping letters and digits\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mUsed stopwords \u001b[36menglish\u001b[0m\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model generated in \u001b[34m3.77\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mLoad 180 stopwords from \u001b[36menglish, stopwords/custom.csv\u001b[0m\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model generated in \u001b[34m5.32\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model stored to \u001b[36mword2vec/wikipedia_300_75.w2v\u001b[0m\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings generated in \u001b[34m11.31\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings generated in \u001b[34m13.96\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings stored to \u001b[36mword2vec/wikipedia_300_75.emb\u001b[0m\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mLoaded \u001b[34m300\u001b[0m examples in \u001b[34m2\u001b[0m categories\n"
                     ]
                 }
             ],
             "source": [
                 "session = load_data(\"data/wikipedia_300.csv.gz\", conf={\n",
                 "    \"preprocess\": \"word2vec\",\n",
                 "    \"w2v_vector_size\": 75,\n",
-                "    \"stopwords\": \"english\",\n",
+                "    \"stopwords\": [\"english\", \"stopwords/custom.csv\"],\n",
                 "    \"clean_text\": \"letters digits\",\n",
                 "})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -94,34 +94,34 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Evaluate model using cross-validation\n",
-                "Build a LinearSVC model and evaluate results using 10-fold cross-validation."
+                "Build a RandomForest model and evaluate results using 10-fold cross-validation."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.16\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m3.02\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>92.67%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.70%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>92.67%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -132,15 +132,15 @@
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>11</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>11</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>94.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>6.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>9</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>91.33%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>8.67%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>13</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -150,15 +150,15 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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1arWBY05fvjhh9sf5P/4/vvvVb58ef33v/+1tv3+++83jDtx4oTOnDmjwMBA636cnJwUFhamgIAABQYG6ujRo+rWrVu+9g/kB4sAARSYbt26qUSJEurYsaO2bdumY8eO6bvvvtPgwYN16tQpSdKQIUP05ptvatWqVfr111/Vv3//W97DHxwcrPDwcL3wwgtatWqVdZvLly+XJJUvX14mk0lr1qzRxYsXlZKSIi8vL0VERGjYsGFatGiRjhw5ovj4eM2ePdu6sK5v37767bff9OqrryohIUEff/yxoqOj83W8lSpV0okTJ7Rs2TIdOXJEs2bNynVBo6urq8LDw7V3715t27ZNgwcP1lNPPaVSpUpJksaNG6fJkydr1qxZOnTokPbt26eoqChNmzYtX/UAt0IAAFBg3N3dtXXrVpUrV05dunRR1apV1bt3b127ds06IzB8+HD16NFD4eHhatCggby8vNS5c+dbbnfu3Lnq2rWr+vfvrypVqujFF19UamqqJKlMmTIaN26cXnvtNQUEBGjgwIGSpDfeeEOjR4/W5MmTVbVqVbVp00Zr165VhQoVJF2/Lv/5559r1apVql27tubNm6dJkybl63g7dOigYcOGaeDAgapTp46+//57jR49+oZxoaGh6tKli9q2batWrVqpVq1aNrf59enTRwsWLFBUVJRq1qypRx99VNHR0dZaAXswWW620gYAANyzmAEAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAP6f5JS+2r8OYa9AAAAAElFTkSuQmCC\n",
+                        "image/png": "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TdOUKVM0evRoNW/eXJMnT1afPn3+9vHnz5+vCRMm6IUXXtDp06dVrlw53X333erYsaMkKTc3V88995xOnTolb29vtW/fXtOnT//bxwUA3D4YAYANRgBgBIwA4PZWuBEAzgIAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAbkUptPnn39e6B127tz5LxcDAABKRqECwMMPP1yonZlMJuXm5v6degAAQAkoVAAwm83FXQcAAChBf2sNQEZGhr3qAAAAJajIASA3N1fjx49XUFCQPD09dfToUUnSmDFj9P7779u9QAAAYH9FDgATJ07UggUL9Prrr6t06dLW9jp16mjevHl2LQ4AABSPIgeARYsW6d1331XPnj3l7Oxsba9Xr54OHTpk1+IAAEDxKHIAOH36tMLDw/O0m81mZWdn26UoAABQvIocAGrVqqVt27blaV+xYoUaNGhgl6IAAEDxKtRpgL/3yiuvKCoqSqdPn5bZbNbKlSuVkJCgRYsWac2aNcVRIwAAsLMijwB06dJFq1evVmxsrDw8PPTKK6/o4MGDWr16tR544IHiqBEAANhZkUcAJOm+++7Txo0b7V0LAAAoIX8pAEjSrl27dPDgQUnX1wU0atTIbkUBAIDiVeQAcOrUKT3++OPasWOHfH19JUmXL1/WPffco2XLlqlSpUr2rhEAANhZkdcA9O/fX9nZ2Tp48KCSk5OVnJysgwcPymw2q3///sVRIwAAsLMijwBs3bpV33zzjSIiIqxtERERmjVrlu677z67FgcAAIpHkUcAgoOD873gT25urgIDA+1SFAAAKF5FDgBvvPGGhgwZol27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qfbt21sfN3XqVC1YsEAffPCBtm/fruTkZP33v/+96XH79Omjjz76SDNnztTBgwf1zjvvyNPTU8HBwfr0008lSQkJCTp79qzeeustSdLkyZO1aNEizZ07Vz/99JNGjBihXr16aevWrZKuB5Vu3bqpU6dO2rNnj/r376+XXnqpyK+Jl5eXFixYoAMHDuitt97Se++9p+nTp9v0OXLkiJYvX67Vq1fryy+/1O7duzVo0CDr9iVLluiVV17RxIkTdfDgQU2aNEljxozRwoULi1wPUCALABRCVFSUpUuXLhaLxWIxm82WjRs3WlxdXS3R0dHW7QEBAZbMzEzrYxYvXmyJiIiwmM1ma1tmZqalTJkylvXr11ssFoulYsWKltdff926PTs721KpUiXrsSwWi+X++++3DBs2zGKxWCwJCQkWSZaNGzfmW+eWLVsskiy//vqrtS0jI8Pi7u5u+eabb2z69uvXz/L4449bLBaLZfTo0ZZatWrZbB81alSeff2RJMt///vfAre/8cYblkaNGlnvjx071uLs7Gw5deqUte2LL76wODk5Wc6ePWuxWCyWqlWrWpYuXWqzn/Hjx1uaNm1qsVgslqSkJIsky+7duws8LvBnWAMAoNDWrFkjT09PZWdny2w264knnlBMTIx1e2RkpM28/969e3XkyBF5eXnZ7CcjI0OJiYlKSUnR2bNnddddd1m3ubi46M4778wzDXDDnj175OzsrPvvv7/QdR85ckTp6el64IEHbNqzsrLUoEEDSdLBgwdt6pCkpk2bFvoYN3z88ceaOXOmEhMTlZaWppycHHl7e9v0CQkJUVBQkM1xzGazEhIS5OXlpcTERPXr109PP/20tU9OTo58fHyKXA9QEAIAgEJr2bKl5syZo9KlSyswMFAuLrZ/Qn7/bW+SlJaWpkaNGmnJkiV59nXHHXf8pRrKlClT5MekpaVJktauXWvzxivJ5lvr/q5vv/1WPXv21Lhx49SuXTv5+Pho2bJlmjp1apFrfe+99/IEEmdnZ7vVChAAABSah4eHwsPDC92/YcOG+vjjj1W+fPk8n4JvqFixor7//ns1b95c0vVPunFxcWrYsGG+/SMjI2U2m7V161a1adMmz/YbIxC5ubnWtlq1asnV1VUnTpwocOSgZs2a1gWNN3z33Xd//iR/55tvvlHlypX173//29p2/PjxPP1OnDihM2fOKDAw0HocJycnRUREKCAgQIGBgTp69Kh69uxZpOMDRcEiQADFpmfPnipXrpy6dOmibdu2KSkpSV999ZWGDh2qU6dOSZKGDRum1157TatWrdKhQ4c0aNCgm57DHxoaqqioKD311FNatWqVdZ/Lly+XJFWuXFkmk0lr1qzRxYsXlZaWJi8vL0VHR2vEiBFauHChEhMTFR8fr1mzZlkX1g0YMEA///yzXnzxRSUkJGjp0qVasGBBkZ5vtWrVdOLECS1btkyJiYmaOXNmvgsa3dzcFBUVpb1792rbtm0aOnSoevTooQoVKkiSxo0bp8mTJ2vmzJk6fPiw9u3bp/nz52vatGlFqge4GQIAgGLj7u6ur7/+WiEhIerWrZtq1qypfv36KSMjwzoi8MILL6h3796KiopS06ZN5eXlpa5du950v3PmzFH37t01aNAg1ahRQ08//bSuXr0qSQoKCtK4ceP00ksvKSAgQIMHD5YkjR8/XmPGjNHkyZNVs2ZNtW/fXmvXrlWVKlUkXZ+X//TTT7Vq1SrVq1dPc+fO1aRJk4r0fDt37qwRI0Zo8ODBql+/vr755huNGTMmT7/w8HB169ZNHTp0UNu2bVW3bl2b0/z69++vefPmaf78+YqMjNT999+vBQsWWGsF7MFkKWilDQAAuG0xAgAAgAERAAAAMCACAAAABkQAAADAgAgAAAAYEAEAAAADIgAAAGBABAAAAAyIAAAAgAERAAAAMCACAAAABvT/WGfe9yXoYKQAAAAASUVORK5CYII=\n",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
@@ -167,28 +167,28 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "evaluate_model(LinearSVC(), session, reload=False, conf={\n",
+                "evaluate_model(RandomForestClassifier(), session, reload=False, conf={\n",
                 "    \"mode\": \"CV-10\",\n",
                 "    \"categories\": True,\n",
                 "    \"confusion_matrix\": True,\n",
                 "    \"seed\": 42,\n",
                 "})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Evaluate model using train-test split\n",
-                "Build a LinearSVC model and evaluate results using train-test split."
+                "Build a RandomForest model and evaluate results using train-test split."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
@@ -213,22 +213,22 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.16\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m2.67\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>92.67%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>93.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.68%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>93.67%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -239,15 +239,15 @@
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>11</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>11</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>94.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>5.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>8</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>11</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -257,15 +257,15 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "evaluate_model(LinearSVC(), session, reload=False, conf={\n",
+                "evaluate_model(RandomForestClassifier(), session, reload=False, conf={\n",
                 "    \"mode\": \"CV-10\",\n",
                 "    \"categories\": True,\n",
                 "    \"seed\": 42,\n",
                 "})"
             ]
         },
         {
@@ -281,21 +281,21 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[36m0.01\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.26\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mExample is predicted as \u001b[32mGames\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
-                "build_model(LinearSVC(), session)\n",
+                "build_model(RandomForestClassifier(), session)\n",
                 "predict(\"This is an article about gamers - people who love playing games\", session)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `mltlk-0.1.2/data/spiral.csv` & `mltlk-0.1.3/data/spiral.csv`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.2/data/wikipedia_300.csv.gz` & `mltlk-0.1.3/data/wikipedia_300.csv.gz`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.2/mltlk/ml.py` & `mltlk-0.1.3/mltlk/ml.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import matplotlib.pyplot as plt
 import re
 from .utils import *
 # Pre-processing
 from sklearn.preprocessing import LabelEncoder
 from sklearn.feature_extraction.text import CountVectorizer, TfidfTransformer
 from sklearn.model_selection import train_test_split
-from nltk.corpus import stopwords
 from sklearn.preprocessing import StandardScaler
 from sklearn.preprocessing import Normalizer
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.preprocessing import OrdinalEncoder
 # Classifiers
 from sklearn.naive_bayes import MultinomialNB
 from sklearn.svm import LinearSVC
@@ -157,31 +156,30 @@
                 xi = xi.lower()
                 # Strip trailing/leading whitespaces
                 xi = xi.strip()
                 session["X"][i] = xi
     
     # Bag-of-words representation for input texts
     if conf["preprocess"] in ["bag-of-words", "bow"]:
+        sw = load_stopwords(conf, verbose=verbose)
+        l = "Used bag-of-words"
         if "stopwords" in conf:
-            sw = list(stopwords.words(conf["stopwords"]))
-            if verbose >= 1:
-                info("Used bag-of-words with stopwords " + colored(conf["stopwords"], "cyan") + " removed")
-        else:
-            sw = None
-            if verbose >= 1:
-                info("Used bag-of-words")
+            l += " with stopwords removed"
+        elif verbose >= 1:
+            l = "Used bag-of-words"
         session["bow"] = CountVectorizer(stop_words=sw).fit(session["X"]) #todo: max_features=max_words, ngram_range=ngram)
         session["X"] = session["bow"].transform(session["X"])
     
         # TF-IDF conversion for bag-of-words
         if "TF-IDF" in conf and conf["TF-IDF"] or "tf-idf" in conf and conf["tf-idf"]:
             session["TF-IDF"] = TfidfTransformer().fit(session["X"])
             session["X"] = session["TF-IDF"].transform(session["X"])
-            if verbose >= 1:
-                info("Used TF-IDF")
+            l += " and TF-IDF"
+        if verbose >= 1:
+            info(l)
     # Word2vec
     if conf["preprocess"] in ["word2vec", "wordtovec"]:
         load_word2vec_data(session, conf, verbose=verbose)
         
     # One-hot encoding
     if conf["preprocess"] in ["one-hot", "onehot", "one hot"]:
         session["scaler"] = OneHotEncoder(handle_unknown="ignore").fit(session["X"])
@@ -641,21 +639,21 @@
         conf["mode"] = "all"
     
     if conf["mode"] in ["train-test", "split"]:
         st = time.time()
         model.fit(session["X_train"], session["y_train"])
         session["model"] = model
         en = time.time()
-        info("Building final model on training data took " + colored(f"{en-st:.2f}", "cyan") + " sec")
+        info("Building final model on training data took " + colored(f"{en-st:.2f}", "blue") + " sec")
     elif conf["mode"] in ["all", ""]:
         st = time.time()
         model.fit(session["X"], session["y"])
         session["model"] = model
         en = time.time()
-        info("Building final model on all data took " + colored(f"{en-st:.2f}", "cyan") + " sec")
+        info("Building final model on all data took " + colored(f"{en-st:.2f}", "blue") + " sec")
     else:
         error("Invalid mode " + colored(conf["mode"], "cyan"))
 
 
 #
 # Save session to file
 #
@@ -665,19 +663,22 @@
         return
     
     # Check if path exists
     fpath = "sessions"
     if not exists(fpath):
         mkdir(fpath)
     
+    # Date-time
+    session["created"] = timestamp_to_str(None)
+    
     # Dump to file
     file = f"sessions/{id}.gz"
     dump(session, gzip.open(file, "wb"))
     if verbose >= 1:
-        info("Session saved to " + colored(file, "blue"))
+        info("Session saved to " + colored(file, "cyan"))
 
 
 #
 # Load session from file
 #
 def load_session(id, verbose=1):
     file = f"sessions/{id}.gz"
@@ -685,15 +686,15 @@
         file += ".gz"
     if not exists(file):
         error("File " + colored(file, "cyan") + " not found")
         return None
     # Load file
     s = load(gzip.open(file, "rb"))
     if verbose >= 1:
-        info("Session loaded from " + colored(file, "blue"))
+        info("Session loaded from " + colored(file, "cyan") + " (created at " + colored(s["created"], "blue") + " from file " + colored(s["file"], "cyan") + ")")
     return s
 
 
 #
 # Dump n prediction errors
 #
 def prediction_errors_for_category(session, category, predicted_category=None, sidx=0, n=5):
```

### Comparing `mltlk-0.1.2/mltlk/resampling.py` & `mltlk-0.1.3/mltlk/resampling.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.2/mltlk/word2vec.py` & `mltlk-0.1.3/mltlk/word2vec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # Basic stuff
 from termcolor import colored
 from .utils import *
 import time
-# Pre-processing
-from nltk.corpus import stopwords
 # Word2Vec
 from gensim.models import Word2Vec
 # File stuff
 from pickle import dump,load
 from os.path import exists
 from os import mkdir
 import gzip
@@ -38,25 +36,26 @@
     if exists(f"word2vec/{fname}") and not conf["rebuild"]:
         wtovec = load(gzip.open(f"word2vec/{fname}", "rb"))
         if verbose >= 1:
             info("Word2vec model loaded from " + colored(f"word2vec/{fname}", "cyan"))
         return wtovec
     
     # Stopwords
-    if "stopwords" in conf:
-        stpwrds = set(stopwords.words(conf["stopwords"]))
-        if verbose >= 1:
-            info("Used stopwords " + colored(conf["stopwords"], "cyan"))
+    sw = load_stopwords(conf, verbose=verbose)
+    if sw is None:
+        sw = set()
+    else:
+        sw = set(sw)
     
     # Convert to list of list of words
     X = []
     for wds in session["X"]:
         xi = []
         for w in wds.split(" "):
-            if w not in stpwrds and w.strip() != "":
+            if w not in sw and w.strip() != "":
                 xi.append(w)
         X.append(xi)
         
     # Update data
     session["X"] = X
     
     # Train Word2Vec model
```


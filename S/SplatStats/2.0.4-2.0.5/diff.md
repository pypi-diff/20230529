# Comparing `tmp/SplatStats-2.0.4.tar.gz` & `tmp/SplatStats-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-2.0.4.tar", last modified: Sat May 20 19:26:40 2023, max compression
+gzip compressed data, was "SplatStats-2.0.5.tar", last modified: Mon May 29 20:06:14 2023, max compression
```

## Comparing `SplatStats-2.0.4.tar` & `SplatStats-2.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-20 19:26:40.936253 SplatStats-2.0.4/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.0.4/LICENSE
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-20 19:26:40.936123 SplatStats-2.0.4/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6368 2023-05-11 17:29:12.000000 SplatStats-2.0.4/README.md
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-20 19:26:40.935107 SplatStats-2.0.4/SplatStats/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/Battle.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/Player.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/StatInk.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/Team.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-05-20 19:26:40.000000 SplatStats-2.0.4/SplatStats/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13972 2023-05-18 20:39:55.000000 SplatStats-2.0.4/SplatStats/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5499 2023-05-16 16:38:00.000000 SplatStats-2.0.4/SplatStats/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/files.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/parsers.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/plotsAux.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/plotsTeam.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10176 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/statInkConstants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10588 2023-05-18 23:06:43.000000 SplatStats-2.0.4/SplatStats/statInkPlots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/statInkStats.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13991 2023-05-11 17:29:12.000000 SplatStats-2.0.4/SplatStats/stats.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-20 19:26:40.935916 SplatStats-2.0.4/SplatStats.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-20 19:26:40.000000 SplatStats-2.0.4/SplatStats.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-05-20 19:26:40.000000 SplatStats-2.0.4/SplatStats.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-05-20 19:26:40.000000 SplatStats-2.0.4/SplatStats.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-05-20 19:26:40.000000 SplatStats-2.0.4/SplatStats.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-05-20 19:26:40.000000 SplatStats-2.0.4/SplatStats.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-05-20 19:26:40.936299 SplatStats-2.0.4/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.0.4/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-29 20:06:14.630329 SplatStats-2.0.5/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.0.5/LICENSE
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-29 20:06:14.629952 SplatStats-2.0.5/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6368 2023-05-11 17:29:12.000000 SplatStats-2.0.5/README.md
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-29 20:06:14.625827 SplatStats-2.0.5/SplatStats/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/Battle.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/Player.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/StatInk.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/Team.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-05-29 20:06:14.000000 SplatStats-2.0.5/SplatStats/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13972 2023-05-18 20:39:55.000000 SplatStats-2.0.5/SplatStats/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5499 2023-05-16 16:38:00.000000 SplatStats-2.0.5/SplatStats/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/files.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/parsers.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/plotsAux.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/plotsTeam.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10176 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/statInkConstants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10588 2023-05-18 23:06:43.000000 SplatStats-2.0.5/SplatStats/statInkPlots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.0.5/SplatStats/statInkStats.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14368 2023-05-29 19:37:30.000000 SplatStats-2.0.5/SplatStats/stats.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-29 20:06:14.629103 SplatStats-2.0.5/SplatStats.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-29 20:06:14.000000 SplatStats-2.0.5/SplatStats.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-05-29 20:06:14.000000 SplatStats-2.0.5/SplatStats.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-05-29 20:06:14.000000 SplatStats-2.0.5/SplatStats.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-05-29 20:06:14.000000 SplatStats-2.0.5/SplatStats.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-05-29 20:06:14.000000 SplatStats-2.0.5/SplatStats.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-05-29 20:06:14.630483 SplatStats-2.0.5/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.0.5/setup.py
```

### Comparing `SplatStats-2.0.4/LICENSE` & `SplatStats-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/PKG-INFO` & `SplatStats-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.0.4
+Version: 2.0.5
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.0.4/README.md` & `SplatStats-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/Battle.py` & `SplatStats-2.0.5/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/Player.py` & `SplatStats-2.0.5/SplatStats/Player.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/StatInk.py` & `SplatStats-2.0.5/SplatStats/StatInk.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/Team.py` & `SplatStats-2.0.5/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/__init__.py` & `SplatStats-2.0.5/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/auxiliary.py` & `SplatStats-2.0.5/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/colors.py` & `SplatStats-2.0.5/SplatStats/colors.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/constants.py` & `SplatStats-2.0.5/SplatStats/constants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/files.py` & `SplatStats-2.0.5/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/parsers.py` & `SplatStats-2.0.5/SplatStats/parsers.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/plots.py` & `SplatStats-2.0.5/SplatStats/plots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/plotsAux.py` & `SplatStats-2.0.5/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/plotsTeam.py` & `SplatStats-2.0.5/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/statInkConstants.py` & `SplatStats-2.0.5/SplatStats/statInkConstants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/statInkPlots.py` & `SplatStats-2.0.5/SplatStats/statInkPlots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/statInkStats.py` & `SplatStats-2.0.5/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/SplatStats/stats.py` & `SplatStats-2.0.5/SplatStats/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,24 +29,35 @@
     (kAvg, dAvg, aAvg, sAvg, pAvg) = [
         i/matchNum for i in (kTot, dTot, aTot, sTot, pTot)
     ]
     kaAvg = (kaTot/matchNum)
     # Win/lose stats (NA are loss) ----------------------------------------
     win  = [True if i=='W' else False for i in bHist['win']]
     wins = sum(win)
-    winR = wins/len(win)
+    winR = (wins/len(win) if len(win) > 0 else 0)
     loss = len(win)-wins
     # Ratios --------------------------------------------------------------
-    killRatio = kTot/dTot
-    kallRatio = kaTot/dTot
+    killRatio = (kTot/dTot if dTot > 0 else 0)
+    kallRatio = (kaTot/dTot if dTot > 0 else 0)
     (kpm, dpm, apm, spm, ppm) = [
-        np.mean(bHist[i]/matchDuration) for i in cats
+        np.mean(
+            np.divide(
+                bHist[i], matchDuration, 
+                out=np.zeros_like(bHist[i]), 
+                where=matchDuration!=0
+            )
+        ) 
+        for i in cats
     ]
     kallpm = np.mean(
-        (bHist['kill']+kassistWeight*bHist['assist'])/matchDuration
+        np.divide(
+            (bHist['kill']+kassistWeight*bHist['assist']), matchDuration, 
+            out=np.zeros_like((bHist['kill']+kassistWeight*bHist['assist'])), 
+            where=matchDuration!=0
+        )
     )
     # Stats dictionary ----------------------------------------------------
     pStats = {
         # W/L stats
         'general': {
             'total matches': matchNum, 'paint': pTot,
             'win': wins, 'loss': loss,
```

### Comparing `SplatStats-2.0.4/SplatStats.egg-info/PKG-INFO` & `SplatStats-2.0.5/SplatStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.0.4
+Version: 2.0.5
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.0.4/SplatStats.egg-info/SOURCES.txt` & `SplatStats-2.0.5/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-2.0.4/setup.py` & `SplatStats-2.0.5/setup.py`

 * *Files identical despite different names*


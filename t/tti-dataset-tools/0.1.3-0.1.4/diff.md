# Comparing `tmp/tti_dataset_tools-0.1.3.tar.gz` & `tmp/tti_dataset_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tti_dataset_tools-0.1.3.tar", max compression
+gzip compressed data, was "tti_dataset_tools-0.1.4.tar", max compression
```

## Comparing `tti_dataset_tools-0.1.3.tar` & `tti_dataset_tools-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,20 @@
--rw-r--r--   0        0        0     1089 2022-12-16 21:14:46.000000 tti_dataset_tools-0.1.3/LICENSE
--rw-r--r--   0        0        0      965 2023-05-12 02:50:22.000000 tti_dataset_tools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       82 2022-12-16 21:14:46.000000 tti_dataset_tools-0.1.3/README.md
--rw-r--r--   0        0        0      245 2023-05-04 17:46:00.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/__init__.py
--rw-r--r--   0        0        0     1012 2023-05-04 17:46:46.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/ColMapper.py
--rw-r--r--   0        0        0     4371 2023-05-04 17:46:00.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/InfluenceAnalyzer.py
--rw-r--r--   0        0        0        0 2023-05-04 17:45:58.510000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/models/__init__.py
--rw-r--r--   0        0        0     6200 2023-05-04 17:46:00.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/models/CrosswalkModel.py
--rw-r--r--   0        0        0     6615 2023-05-12 02:43:16.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryCleaner.py
--rw-r--r--   0        0        0     1179 2023-05-04 17:46:06.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryProcessor.py
--rw-r--r--   0        0        0     9161 2023-05-04 17:47:00.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryTransformer.py
--rw-r--r--   0        0        0     1350 2023-05-04 17:46:06.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryVisualizer.py
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.3/setup.py
--rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2022-12-16 21:14:46.000000 tti_dataset_tools-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1058 2023-05-28 23:23:22.000000 tti_dataset_tools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       82 2022-12-16 21:14:46.000000 tti_dataset_tools-0.1.4/README.md
+-rw-r--r--   0        0        0       42 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.4/src/ind_tools/__init__.py
+-rw-r--r--   0        0        0     1471 2023-05-28 23:36:30.000000 tti_dataset_tools-0.1.4/src/ind_tools/IndTransformer.py
+-rw-r--r--   0        0        0      303 2023-05-28 23:13:00.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/__init__.py
+-rw-r--r--   0        0        0     1012 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/ColMapper.py
+-rw-r--r--   0        0        0     4371 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/InfluenceAnalyzer.py
+-rw-r--r--   0        0        0        0 2023-05-04 17:45:58.510000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/models/__init__.py
+-rw-r--r--   0        0        0     6200 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/models/CrosswalkModel.py
+-rw-r--r--   0        0        0     1123 2023-05-28 23:07:06.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrackClass.py
+-rw-r--r--   0        0        0      470 2023-05-28 23:03:20.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrackDirection.py
+-rw-r--r--   0        0        0     6615 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrajectoryCleaner.py
+-rw-r--r--   0        0        0     2017 2023-05-28 23:21:04.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrajectoryMetaBuilder.py
+-rw-r--r--   0        0        0     1215 2023-05-28 23:15:48.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrajectoryProcessor.py
+-rw-r--r--   0        0        0    10468 2023-05-28 23:34:46.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrajectoryTransformer.py
+-rw-r--r--   0        0        0    19059 2023-05-28 23:03:34.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrajectoryUtils.py
+-rw-r--r--   0        0        0     2314 2023-05-28 22:58:02.000000 tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrajectoryVisualizer.py
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.4/setup.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.4/PKG-INFO
```

### Comparing `tti_dataset_tools-0.1.3/LICENSE` & `tti_dataset_tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.3/pyproject.toml` & `tti_dataset_tools-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [tool.poetry]
 name = "tti-dataset-tools"
-version = "0.1.3"
+version = "0.1.4"
 description = "A set of tools for trajectory dataset transformation, clean-up, and augmentation"
 authors = ["Golam Md Muktadir <muktadir@ucsc.edu>"]
 license = "Mozilla Public License Version 2.0"
 include = [
     "MIT License",
 ]
 
 homepage = "https://github.com/adhocmaster/TTI-dataset-tools"
 repository = "https://github.com/adhocmaster/TTI-dataset-tools"
 keywords = ["Trajectory Dataset", "Trajectory Analysis", "Trajectory Transformation", "Trajectory Augmentation"]
 
 readme = "README.md"
-packages = [{include = "tti_dataset_tools", from="./src"}]
+packages = [{include = "tti_dataset_tools", from="./src"}, {include = "ind_tools", from="./src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 pandas = "^1.5.2"
 numpy = "^1.20.3"
 shapely = "~1.7.1"
+seaborn = "~0.12.1"
+tqdm = "^4.65.0"
+vg = "^2.0.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^3.5.2"
```

### Comparing `tti_dataset_tools-0.1.3/src/tti_dataset_tools/ColMapper.py` & `tti_dataset_tools-0.1.4/src/tti_dataset_tools/ColMapper.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.3/src/tti_dataset_tools/InfluenceAnalyzer.py` & `tti_dataset_tools-0.1.4/src/tti_dataset_tools/InfluenceAnalyzer.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.3/src/tti_dataset_tools/models/CrosswalkModel.py` & `tti_dataset_tools-0.1.4/src/tti_dataset_tools/models/CrosswalkModel.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryCleaner.py` & `tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrajectoryCleaner.py`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryProcessor.py` & `tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrajectoryProcessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .ColMapper import ColMapper
 
 class TrajectoryProcessor:
 
     def __init__(self,
             colMapper: ColMapper
         ):
+        self.colMapper = colMapper
         self.idCol = colMapper.idCol
         self.xCol = colMapper.xCol
         self.yCol = colMapper.yCol
         self.xVelCol = colMapper.xVelCol
         self.yVelCol = colMapper.yVelCol
         self.speedCol = colMapper.speedCol
         self.fps = colMapper.fps
```

### Comparing `tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryTransformer.py` & `tti_dataset_tools-0.1.4/src/tti_dataset_tools/TrajectoryTransformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pandas as pd
 from typing import *
 import math
 from .ColMapper import ColMapper
 from .TrajectoryProcessor import TrajectoryProcessor
+from .TrajectoryMetaBuilder import TrajectoryMetaBuilder
 
 class TrajectoryTransformer(TrajectoryProcessor):
 
     def __init__(self,
             colMapper: ColMapper
         ):
         
@@ -219,53 +220,85 @@
         
         firstRow = trackDf.iloc[0]
         if firstRow[self.displacementXCol] != 0.0 or firstRow[self.displacementYCol] != 0.0:
             raise Exception(f"track {firstRow[self.idCol]} has incorrect local source displacement {firstRow[self.displacementXCol]}, {firstRow[self.displacementYCol]}")
         
         
 
-    def rotate(self, trackDf: pd.DataFrame) -> Tuple[pd.Series, pd.Series]:
+    def rotate(self, trackDf: pd.DataFrame, xCol: str, yCol: str) -> Tuple[pd.Series, pd.Series]:
         """rotation is y=-y and x=-x. Does inplace transformation on localX, localY
 
         Args:
             trackDf (pd.DataFrame): A single track
         """
 
         raise NotImplemented("Not implemented error")
     
-    def rotate180(self, trackDf: pd.DataFrame) -> Tuple[pd.Series, pd.Series]:
+    def rotate180(self, trackDf: pd.DataFrame, xCol: str, yCol: str) -> Tuple[pd.Series, pd.Series]:
         """rotation is y=-y and x=-x. Does inplace transformation on localX, localY
 
         Args:
             trackDf (pd.DataFrame): A single track
         """
 
-        X = -trackDf[self.localXCol]
-        Y = -trackDf[self.localYCol]
+        X = -trackDf[xCol]
+        Y = -trackDf[yCol]
 
         return X, Y
+    
 
-    def flipAlongY(self, trackDf: pd.DataFrame):
+    def flipAlongY(self, trackDf: pd.DataFrame, xCol: str, yCol: str):
         """Flips along the y axis (negates x coordinates). Does inplace transformation on localX, localY
 
         Args:
             trackDf (pd.DataFrame): A single track
 
         """
         # TODO
         
         pass
 
-    def flipAlongX(self, trackDf: pd.DataFrame):
+    def flipAlongX(self, trackDf: pd.DataFrame, xCol: str, yCol: str):
         """Flips along the x axis (negates y coordinates). Does inplace transformation on localX, localY
 
         Args:
             trackDf (pd.DataFrame): A single track
 
         """
         # TODO
         pass
 
+
+    # region direction transfomations
+    def convertTracksToNorth(self,
+            tracksDf:pd.DataFrame,
+            xCol: str,
+            yCol: str,
+            tracksMeta: pd.DataFrame = None,
+        ) -> Tuple[List[int], pd.DataFrame]:
+        
+        if tracksMeta is None:
+            metaBuilder = TrajectoryMetaBuilder(self.colMapper)
+            tracksMeta = metaBuilder.build([tracksDf], xCol, yCol)
+
+        copiedDf = tracksDf.copy()
+        allPedIds = self.getIds(copiedDf)
+
+        southIds = []
+        for pedId in allPedIds:
+            trackDf = copiedDf[copiedDf[self.idCol] == pedId]
+            trackMeta = self.getMeta(tracksMeta, pedId)
+            # print(trackMeta[self.verticalDirectionCol])
+            if trackMeta[self.verticalDirectionCol] == "SOUTH":
+                southIds.append(pedId)
+                # print(trackMeta[self.idCol])
+                X, Y = self.rotate180(trackDf, xCol=xCol, yCol=yCol)
+                copiedDf.loc[copiedDf[self.idCol] == pedId, xCol] = X
+                copiedDf.loc[copiedDf[self.idCol] == pedId, yCol] = Y
+        
+        return southIds, copiedDf
+    # endregion
+
```

### Comparing `tti_dataset_tools-0.1.3/setup.py` & `tti_dataset_tools-0.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
-{'': 'src'}
+{'': 'src', 'ind_tools': 'src\\ind_tools'}
 
 packages = \
-['tti_dataset_tools', 'tti_dataset_tools.models']
+['ind_tools', 'tti_dataset_tools', 'tti_dataset_tools.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.20.3,<2.0.0', 'pandas>=1.5.2,<2.0.0', 'shapely>=1.7.1,<1.8.0']
+['numpy>=1.20.3,<2.0.0',
+ 'pandas>=1.5.2,<2.0.0',
+ 'seaborn>=0.12.1,<0.13.0',
+ 'shapely>=1.7.1,<1.8.0',
+ 'tqdm>=4.65.0,<5.0.0',
+ 'vg>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'tti-dataset-tools',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'A set of tools for trajectory dataset transformation, clean-up, and augmentation',
     'long_description': '# A set of tools for trajectory dataset transformation, clean-up, and augmentation',
     'author': 'Golam Md Muktadir',
     'author_email': 'muktadir@ucsc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/adhocmaster/TTI-dataset-tools',
```

### Comparing `tti_dataset_tools-0.1.3/PKG-INFO` & `tti_dataset_tools-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tti-dataset-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of tools for trajectory dataset transformation, clean-up, and augmentation
 Home-page: https://github.com/adhocmaster/TTI-dataset-tools
 License: Mozilla Public License Version 2.0
 Keywords: Trajectory Dataset,Trajectory Analysis,Trajectory Transformation,Trajectory Augmentation
 Author: Golam Md Muktadir
 Author-email: muktadir@ucsc.edu
 Requires-Python: >=3.8.0,<4.0.0
@@ -12,12 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.20.3,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: seaborn (>=0.12.1,<0.13.0)
 Requires-Dist: shapely (>=1.7.1,<1.8.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: vg (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/adhocmaster/TTI-dataset-tools
 Description-Content-Type: text/markdown
 
 # A set of tools for trajectory dataset transformation, clean-up, and augmentation
```


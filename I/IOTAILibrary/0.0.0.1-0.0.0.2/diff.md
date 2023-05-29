# Comparing `tmp/IOTAILibrary-0.0.0.1-py3-none-any.whl.zip` & `tmp/IOTAILibrary-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6611 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     9266 b- defN 23-May-29 17:15 Data/IOTDataProcessor.py
--rw-rw-rw-  2.0 fat     1391 b- defN 22-Nov-29 15:30 Data/IOTDataStructure.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-10 16:28 Data/__init__.py
--rw-rw-rw-  2.0 fat     7634 b- defN 23-Jan-11 16:15 Model/IOTModelGenerator.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-10 16:28 Model/__init__.py
--rw-rw-rw-  2.0 fat      470 b- defN 23-May-29 17:16 IOTAILibrary-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 17:16 IOTAILibrary-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-May-29 17:16 IOTAILibrary-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      711 b- defN 23-May-29 17:16 IOTAILibrary-0.0.0.1.dist-info/RECORD
-9 files, 19575 bytes uncompressed, 5379 bytes compressed:  72.5%
+Zip file size: 6597 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     9262 b- defN 23-May-29 17:21 IOTData/Processor.py
+-rw-rw-rw-  2.0 fat     1391 b- defN 22-Nov-29 15:30 IOTData/Structure.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-10 16:28 IOTData/__init__.py
+-rw-rw-rw-  2.0 fat     7630 b- defN 23-May-29 17:21 IOTModel/Generator.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-10 16:28 IOTModel/__init__.py
+-rw-rw-rw-  2.0 fat      470 b- defN 23-May-29 17:23 IOTAILibrary-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 17:23 IOTAILibrary-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-29 17:23 IOTAILibrary-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      704 b- defN 23-May-29 17:23 IOTAILibrary-0.0.0.2.dist-info/RECORD
+9 files, 19566 bytes uncompressed, 5379 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: Data/IOTDataProcessor.py
+Filename: IOTData/Processor.py
 Comment: 
 
-Filename: Data/IOTDataStructure.py
+Filename: IOTData/Structure.py
 Comment: 
 
-Filename: Data/__init__.py
+Filename: IOTData/__init__.py
 Comment: 
 
-Filename: Model/IOTModelGenerator.py
+Filename: IOTModel/Generator.py
 Comment: 
 
-Filename: Model/__init__.py
+Filename: IOTModel/__init__.py
 Comment: 
 
-Filename: IOTAILibrary-0.0.0.1.dist-info/METADATA
+Filename: IOTAILibrary-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: IOTAILibrary-0.0.0.1.dist-info/WHEEL
+Filename: IOTAILibrary-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: IOTAILibrary-0.0.0.1.dist-info/top_level.txt
+Filename: IOTAILibrary-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: IOTAILibrary-0.0.0.1.dist-info/RECORD
+Filename: IOTAILibrary-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Data/IOTDataProcessor.py` & `IOTData/Processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import Data.IOTDataStructure as dt
+import IOTData.Structure as dt
 import matplotlib.pyplot as plt
 import seaborn as seaborn_plotter
 import pandas as pd
 import numpy as np
 import random as rdn
 import os as _os
```

## Comparing `Data/IOTDataStructure.py` & `IOTData/Structure.py`

 * *Files identical despite different names*

## Comparing `Model/IOTModelGenerator.py` & `IOTModel/Generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from tensorflow.keras.models import Sequential
 from tensorflow.keras.layers import Dense
 from tensorflow.keras.utils import to_categorical
 from tensorflow.keras.layers import Dense, Dropout, Activation, Flatten
 from tensorflow.keras.optimizers import SGD
 from sklearn.model_selection import train_test_split
 from tensorflow import keras
-import Data.IOTDataStructure as dt
+import IOTData.Structure as dt
 import os as _os
 
 class IOTModelGenerator(object):
     """description of class"""
 
     def __init__(self):
         print("Initial Model Generator")
```


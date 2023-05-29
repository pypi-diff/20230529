# Comparing `tmp/mcnets-0.2.5.tar.gz` & `tmp/mcnets-0.2.6.tar.gz`

## Comparing `mcnets-0.2.5.tar` & `mcnets-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,39 @@
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 mcnets-0.2.5/Tests Journal.txt
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 mcnets-0.2.5/Updates.txt
--rw-r--r--   0        0        0    17375 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/Fit 1 (default method, net as function).png
--rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/Fit 2 (net as derivative, holy cow!).png
--rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/Fit 3 (Another new attempt).png
--rw-r--r--   0        0        0    39485 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/Moar custom architecture tests.JPG
--rw-r--r--   0        0        0    45066 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (100x100, n=1).png
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (40x40, n=1).png
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (50x50 n=1).png
--rw-r--r--   0        0        0    12524 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (50x50 n=100).png
--rw-r--r--   0        0        0    12798 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (50x50 n=20).png
--rw-r--r--   0        0        0    43952 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (75x75, n=1).png
--rw-r--r--   0        0        0    53568 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes with 6.5-8.5k parameter line (75x75, n=1).png
--rw-r--r--   0        0        0    51028 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes with 9-11k parameter line (75x75, n=1).png
--rw-r--r--   0        0        0    34666 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/genTrain 1 (Holy cow i can do sin now!).png
--rw-r--r--   0        0        0    32480 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/genTrain 2 (sin pt.2 with a 50x15 ATAN net).png
--rw-r--r--   0        0        0    30412 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/genTrain 3 (20 points, R2 = 0.848).png
--rw-r--r--   0        0        0    16692 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/genTrain 4 (10 points, R2 = 0.998880, #params=44960, and use the true indicies!).png
--rw-r--r--   0        0        0    18779 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/genTrain 5 (10 points, R2 = 0.993114, #params=4920, and use the true indicies!).png
--rw-r--r--   0        0        0    17375 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/ghFit1.png
--rw-r--r--   0        0        0    15854 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/ghFit1a.png
--rw-r--r--   0        0        0    17039 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/ghFit1b.png
--rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/ghFit2.png
--rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/ghFit2b.png
--rw-r--r--   0        0        0    15211 2020-02-02 00:00:00.000000 mcnets-0.2.5/GraphPicStuff/ghSpeedTest1a.png
--rw-r--r--   0        0        0    38000 2020-02-02 00:00:00.000000 mcnets-0.2.5/src/mcnets/Feature Experiments.ipynb
--rw-r--r--   0        0        0    21238 2020-02-02 00:00:00.000000 mcnets-0.2.5/src/mcnets/Github Example.ipynb
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mcnets-0.2.5/src/mcnets/__init__.py
--rw-r--r--   0        0        0    50123 2020-02-02 00:00:00.000000 mcnets-0.2.5/src/mcnets/main.py
--rw-r--r--   0        0        0    70272 2020-02-02 00:00:00.000000 mcnets-0.2.5/tests/Slope Fitting.ipynb
--rw-r--r--   0        0        0    74573 2020-02-02 00:00:00.000000 mcnets-0.2.5/tests/Speed Tests.ipynb
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mcnets-0.2.5/LICENSE
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mcnets-0.2.5/README.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 mcnets-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 mcnets-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 mcnets-0.2.6/Tests Journal.txt
+-rw-r--r--   0        0        0     5430 2020-02-02 00:00:00.000000 mcnets-0.2.6/Updates.txt
+-rw-r--r--   0        0        0    17375 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/Fit 1 (default method, net as function).png
+-rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/Fit 2 (net as derivative, holy cow!).png
+-rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/Fit 3 (Another new attempt).png
+-rw-r--r--   0        0        0    39485 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/Moar custom architecture tests.JPG
+-rw-r--r--   0        0        0    45066 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (100x100, n=1).png
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (40x40, n=1).png
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (50x50 n=1).png
+-rw-r--r--   0        0        0    12524 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (50x50 n=100).png
+-rw-r--r--   0        0        0    12798 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (50x50 n=20).png
+-rw-r--r--   0        0        0    43952 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (75x75, n=1).png
+-rw-r--r--   0        0        0    53568 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes with 6.5-8.5k parameter line (75x75, n=1).png
+-rw-r--r--   0        0        0    51028 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes with 9-11k parameter line (75x75, n=1).png
+-rw-r--r--   0        0        0    34666 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/genTrain 1 (Holy cow i can do sin now!).png
+-rw-r--r--   0        0        0    32480 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/genTrain 2 (sin pt.2 with a 50x15 ATAN net).png
+-rw-r--r--   0        0        0    30412 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/genTrain 3 (20 points, R2 = 0.848).png
+-rw-r--r--   0        0        0    16692 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/genTrain 4 (10 points, R2 = 0.998880, #params=44960, and use the true indicies!).png
+-rw-r--r--   0        0        0    18779 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/genTrain 5 (10 points, R2 = 0.993114, #params=4920, and use the true indicies!).png
+-rw-r--r--   0        0        0    17375 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/ghFit1.png
+-rw-r--r--   0        0        0    15854 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/ghFit1a.png
+-rw-r--r--   0        0        0    17039 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/ghFit1b.png
+-rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/ghFit2.png
+-rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/ghFit2b.png
+-rw-r--r--   0        0        0    15211 2020-02-02 00:00:00.000000 mcnets-0.2.6/GraphPicStuff/ghSpeedTest1a.png
+-rw-r--r--   0        0        0    39474 2020-02-02 00:00:00.000000 mcnets-0.2.6/src/mcnets/Feature Experiments.ipynb
+-rw-r--r--   0        0        0    21238 2020-02-02 00:00:00.000000 mcnets-0.2.6/src/mcnets/Github Example.ipynb
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mcnets-0.2.6/src/mcnets/__init__.py
+-rw-r--r--   0        0        0    50105 2020-02-02 00:00:00.000000 mcnets-0.2.6/src/mcnets/main.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mcnets-0.2.6/src/mcnets/MCNetData/NN_Test1_Activations
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 mcnets-0.2.6/src/mcnets/MCNetData/NN_Test1_Size
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mcnets-0.2.6/src/mcnets/MCNetData/NN_Test1_Weights1
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 mcnets-0.2.6/src/mcnets/MCNetData/NN_Test1_Weights2
+-rw-r--r--   0        0        0    70272 2020-02-02 00:00:00.000000 mcnets-0.2.6/tests/Slope Fitting.ipynb
+-rw-r--r--   0        0        0    74573 2020-02-02 00:00:00.000000 mcnets-0.2.6/tests/Speed Tests.ipynb
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mcnets-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mcnets-0.2.6/README.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 mcnets-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 mcnets-0.2.6/PKG-INFO
```

### Comparing `mcnets-0.2.5/Tests Journal.txt` & `mcnets-0.2.6/Tests Journal.txt`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/Updates.txt` & `mcnets-0.2.6/Updates.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 - Add monte-carlo tree search as another advanced training method (might not be worth it?)
 	- Like genTrain, but continues testing a few routes for more than one depth
 - Do test on all acti function combinations for curve fitting test (sin(x+4) - (x^2/10) + x) xE[0,11]
 - Fix training with biases included in .Calculate()
 - Add "Calculation Time" to model __str__ stuff
 
 
+V0.2.6 (Hotfix)
+- Still encountering file errors
+	- Removed the "./" infront of the paths when saving/loading
+	- Commented out "name = str(name)" in LoadNet and SaveNN
+
+
 V0.2.5 (Stupidity Fix)
 - Deleted old_versions from local area
 	- Was creating an exponential file size increase whoops
 	- Just retrieve old versions from PyPI if for some reason needed
 
 
 V0.2.4 (Hotfix)
```

### Comparing `mcnets-0.2.5/GraphPicStuff/Fit 1 (default method, net as function).png` & `mcnets-0.2.6/GraphPicStuff/Fit 1 (default method, net as function).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/Fit 2 (net as derivative, holy cow!).png` & `mcnets-0.2.6/GraphPicStuff/Fit 2 (net as derivative, holy cow!).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/Fit 3 (Another new attempt).png` & `mcnets-0.2.6/GraphPicStuff/Fit 3 (Another new attempt).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/Moar custom architecture tests.JPG` & `mcnets-0.2.6/GraphPicStuff/Moar custom architecture tests.JPG`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (100x100, n=1).png` & `mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (100x100, n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (40x40, n=1).png` & `mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (40x40, n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (50x50 n=1).png` & `mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (50x50 n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (50x50 n=100).png` & `mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (50x50 n=100).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (50x50 n=20).png` & `mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (50x50 n=20).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes (75x75, n=1).png` & `mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes (75x75, n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes with 6.5-8.5k parameter line (75x75, n=1).png` & `mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes with 6.5-8.5k parameter line (75x75, n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/NN Speed vs Sizes with 9-11k parameter line (75x75, n=1).png` & `mcnets-0.2.6/GraphPicStuff/NN Speed vs Sizes with 9-11k parameter line (75x75, n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/genTrain 1 (Holy cow i can do sin now!).png` & `mcnets-0.2.6/GraphPicStuff/genTrain 1 (Holy cow i can do sin now!).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/genTrain 2 (sin pt.2 with a 50x15 ATAN net).png` & `mcnets-0.2.6/GraphPicStuff/genTrain 2 (sin pt.2 with a 50x15 ATAN net).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/genTrain 3 (20 points, R2 = 0.848).png` & `mcnets-0.2.6/GraphPicStuff/genTrain 3 (20 points, R2 = 0.848).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/genTrain 4 (10 points, R2 = 0.998880, #params=44960, and use the true indicies!).png` & `mcnets-0.2.6/GraphPicStuff/genTrain 4 (10 points, R2 = 0.998880, #params=44960, and use the true indicies!).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/genTrain 5 (10 points, R2 = 0.993114, #params=4920, and use the true indicies!).png` & `mcnets-0.2.6/GraphPicStuff/genTrain 5 (10 points, R2 = 0.993114, #params=4920, and use the true indicies!).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/ghFit1.png` & `mcnets-0.2.6/GraphPicStuff/ghFit1.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/ghFit1a.png` & `mcnets-0.2.6/GraphPicStuff/ghFit1a.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/ghFit1b.png` & `mcnets-0.2.6/GraphPicStuff/ghFit1b.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/ghFit2.png` & `mcnets-0.2.6/GraphPicStuff/ghFit2.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/ghFit2b.png` & `mcnets-0.2.6/GraphPicStuff/ghFit2b.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/GraphPicStuff/ghSpeedTest1a.png` & `mcnets-0.2.6/GraphPicStuff/ghSpeedTest1a.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/src/mcnets/Feature Experiments.ipynb` & `mcnets-0.2.6/src/mcnets/Feature Experiments.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9515625%*

 * *Differences: {"'cells'": "{0: {'execution_count': 2}, insert: [(5, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', 1), ('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            "['from main import *'])])), (6, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', 6), ('metadata', OrderedDict()), ('outputs', "*

 * *            "[OrderedDict([('name', 'stdout'), ('output_type', 'stream'), ('text', "*

 * *            "['============================================================= […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "from main import *\n",
                 "import numpy as np\n",
                 "import random as rn\n",
@@ -225,14 +225,71 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model.Calculate(X[0])"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from main import *"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "================================================================\n",
+                        "                  Neural Net Characteristics:                   \n",
+                        "1. Layer Sizes = [1, 3, 1]\n",
+                        "2. Weight Medians = [-0.38, -0.1]\n",
+                        "3. Number of Parameters: 6\n",
+                        "4. Activation Functions: ['RELU', 'RELU']\n",
+                        "================================================================\n"
+                    ]
+                }
+            ],
+            "source": [
+                "nn = AdvNet(1, [3], 1, \"RELU\")\n",
+                "print(nn)\n",
+                "nn.SaveNN(\"Test1\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "================================================================\n",
+                        "                  Neural Net Characteristics:                   \n",
+                        "1. Layer Sizes = [1, 3, 1]\n",
+                        "2. Weight Medians = [-0.38, -0.1]\n",
+                        "3. Number of Parameters: 6\n",
+                        "4. Activation Functions: ['RELU', 'RELU']\n",
+                        "================================================================\n"
+                    ]
+                }
+            ],
+            "source": [
+                "print(LoadNet(\"Test1\"))"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `mcnets-0.2.5/src/mcnets/Github Example.ipynb` & `mcnets-0.2.6/src/mcnets/Github Example.ipynb`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/src/mcnets/main.py` & `mcnets-0.2.6/src/mcnets/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,23 +343,23 @@
 
         # Check that the directory exists
         DIR = "MCNetData"
         if not os.path.exists(DIR):
             os.makedirs(DIR)
 
         # Save the various Characteristics and weights of the NN to load later
-        name = str(name)
-        np.savetxt(f"./{DIR}/NN_{name}_Size", self.sizes)
+        # name = str(name)
+        np.savetxt(f"{DIR}/NN_{name}_Size", self.sizes)
         for i in range(len(self.sizes) - 1):
             # Redundant save cycles in case of 'onedrive' situations
             ## Limit save tries to 10 times, if thats not working
             ## something else is likely wrong that this won't fix
             for tries in range(10):
                 try:
-                    np.savetxt(f"./{DIR}/NN_{name}_Weights{i+1}", self.weights[i])
+                    np.savetxt(f"{DIR}/NN_{name}_Weights{i+1}", self.weights[i])
                     # if made this far, it successfully saved so break the loop
                     break
                 except:
                     # Something didn't work, try again
                     # BTW a 'onedrive' issue is when the local net files
                     # are saved on some cloud-like thing and if saved or
                     # accessed too quickly, will throw a 'permission denied'
@@ -382,62 +382,61 @@
                 data.append(3)
             else:
                 data.append(0)
 
         # Save the activation function information
         for tries in range(10):
             try:
-                np.savetxt(f"./{DIR}/NN_{name}_Activations", np.array(data))
+                np.savetxt(f"{DIR}/NN_{name}_Activations", np.array(data))
                 break
             except:
                 continue
 
     def ApplyTweak(self, dW):
         for i, dWi in enumerate(dW):
             self.weights[i] = self.weights[i] + dWi
 
 ## External Functions ##
-def LoadNet(name):
+def LoadNet(name:str):
     """
     Returns a nerual net object with the loaded characteristics from the
     given nickname. 
     
     Inputs:
 
     1 - Name
     - Type == String
-
     """
 
     # Check that the mcnet data directory exsits
     # If not, make the folder and raise error
     DIR = "MCNetData"
     if not os.path.exists(DIR):
         os.makedirs(DIR)
         raise NotADirectoryError(
             "The net data folder (MCNetData) was not found! It is now made; resave or move existing nets into this folder."
             )
 
     # Load the various Characteristics and weights of the NN
-    name = str(name)
-    for tries in range(10): ## Redundant loading loop, reference SaveNN on 'onedrive issue'
+    # name = str(name)
+    for _ in range(10): ## Redundant loading loop, reference SaveNN on 'onedrive issue'
         try:
-            sizes = list(np.loadtxt(f"./{DIR}/NN_{name}_Size"))
+            sizes = list(np.loadtxt(f"{DIR}/NN_{name}_Size"))
             break
         except:
             continue
     sizes = [int(i) for i in sizes]
     inSize = int(sizes[0])
     hiddenSize = sizes[1:len(sizes)-1]
     outSize = int(sizes[-1])
 
     # Load in the activation function data
-    for tries in range(10): ## Redundant loading loop, reference SaveNN on 'onedrive issue'
+    for _ in range(10): ## Redundant loading loop, reference SaveNN on 'onedrive issue'
         try:
-            activations = list(np.loadtxt(f"./{DIR}/NN_{name}_Activations"))
+            activations = list(np.loadtxt(f"{DIR}/NN_{name}_Activations"))
             break
         except:
             continue
 
     # Convert to str activation data
     strActivations = []
     for function in activations:
@@ -454,17 +453,17 @@
             strActivations.append("NONE")
 
     # From the size, construct the net frame
     net = AdvNet(inSize, hiddenSize, outSize, strActivations)
 
     # Load in the saved net weights
     for i in range(len(net.sizes) - 1):
-        for tries in range(10): ## Redundant loading loop, reference SaveNN on 'onedrive issue'
+        for _ in range(10): ## Redundant loading loop, reference SaveNN on 'onedrive issue'
             try:
-                weights = np.loadtxt(f"./{DIR}/NN_{name}_Weights{i+1}")
+                weights = np.loadtxt(f"{DIR}/NN_{name}_Weights{i+1}")
                 break
             except:
                 continue
         weights = weights.reshape(net.sizes[i], net.sizes[i+1])
         net.weights[i] = weights
 
     # Return the generated neural net
```

### Comparing `mcnets-0.2.5/tests/Slope Fitting.ipynb` & `mcnets-0.2.6/tests/Slope Fitting.ipynb`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/tests/Speed Tests.ipynb` & `mcnets-0.2.6/tests/Speed Tests.ipynb`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/LICENSE` & `mcnets-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/README.md` & `mcnets-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.5/pyproject.toml` & `mcnets-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "matplotlib", "numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mcnets"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Sean", email="svs.2k15@gmail.com" },
 ]
 description = "A package that demonstrates deep neural nets using Monte Carlo-type random parameter training."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mcnets-0.2.5/PKG-INFO` & `mcnets-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcnets
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package that demonstrates deep neural nets using Monte Carlo-type random parameter training.
 Project-URL: Homepage, https://github.com/SciCapt/Monte-Carlo-Neural-Nets
 Project-URL: Bug Tracker, https://github.com/SciCapt/Monte-Carlo-Neural-Nets/issues
 Author-email: Sean <svs.2k15@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


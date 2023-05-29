# Comparing `tmp/ajm1102pandemic2d-0.4-py3-none-any.whl.zip` & `tmp/ajm1102pandemic2d-0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 7283 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       47 b- defN 23-May-29 19:26 ajm1102pandemic2d/__init__.py
--rw-rw-rw-  2.0 fat       41 b- defN 23-May-29 19:00 ajm1102pandemic2d/boundary_class.py
--rw-rw-rw-  2.0 fat     2471 b- defN 23-May-29 18:57 ajm1102pandemic2d/person_class.py
+Zip file size: 7577 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat       45 b- defN 23-May-29 19:48 ajm1102pandemic2d/__init__.py
+-rw-rw-rw-  2.0 fat       41 b- defN 23-May-29 19:35 ajm1102pandemic2d/boundary_class.py
+-rw-rw-rw-  2.0 fat      254 b- defN 23-May-29 19:45 ajm1102pandemic2d/functions.py
+-rw-rw-rw-  2.0 fat     2528 b- defN 23-May-29 19:44 ajm1102pandemic2d/person_class.py
 -rw-rw-rw-  2.0 fat     7453 b- defN 23-May-29 18:59 ajm1102pandemic2d/simulation.py
--rw-rw-rw-  2.0 fat     7453 b- defN 23-May-29 18:59 ajm1102pandemic2d/simulation_class.py
+-rw-rw-rw-  2.0 fat     7234 b- defN 23-May-29 19:46 ajm1102pandemic2d/simulation_class.py
 -rw-rw-rw-  2.0 fat       89 b- defN 23-May-29 18:59 ajm1102pandemic2d/virus_class.py
--rw-rw-rw-  2.0 fat      288 b- defN 23-May-29 19:29 ajm1102pandemic2d-0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 19:29 ajm1102pandemic2d-0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-May-29 19:29 ajm1102pandemic2d-0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      862 b- defN 23-May-29 19:29 ajm1102pandemic2d-0.4.dist-info/RECORD
-10 files, 18814 bytes uncompressed, 5787 bytes compressed:  69.2%
+-rw-rw-rw-  2.0 fat      288 b- defN 23-May-29 19:49 ajm1102pandemic2d-0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 19:49 ajm1102pandemic2d-0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-29 19:49 ajm1102pandemic2d-0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      948 b- defN 23-May-29 19:49 ajm1102pandemic2d-0.5.dist-info/RECORD
+11 files, 18990 bytes uncompressed, 5945 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: ajm1102pandemic2d/__init__.py
 Comment: 
 
 Filename: ajm1102pandemic2d/boundary_class.py
 Comment: 
 
+Filename: ajm1102pandemic2d/functions.py
+Comment: 
+
 Filename: ajm1102pandemic2d/person_class.py
 Comment: 
 
 Filename: ajm1102pandemic2d/simulation.py
 Comment: 
 
 Filename: ajm1102pandemic2d/simulation_class.py
 Comment: 
 
 Filename: ajm1102pandemic2d/virus_class.py
 Comment: 
 
-Filename: ajm1102pandemic2d-0.4.dist-info/METADATA
+Filename: ajm1102pandemic2d-0.5.dist-info/METADATA
 Comment: 
 
-Filename: ajm1102pandemic2d-0.4.dist-info/WHEEL
+Filename: ajm1102pandemic2d-0.5.dist-info/WHEEL
 Comment: 
 
-Filename: ajm1102pandemic2d-0.4.dist-info/top_level.txt
+Filename: ajm1102pandemic2d-0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ajm1102pandemic2d-0.4.dist-info/RECORD
+Filename: ajm1102pandemic2d-0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ajm1102pandemic2d/__init__.py

```diff
@@ -1,4 +1,3 @@
 
-from simulation_class import simulation
-
 
+from simulation_class import simulation
```

## ajm1102pandemic2d/person_class.py

```diff
@@ -1,9 +1,11 @@
+import numpy as np
 from virus_class import virus
-from boundary_class import boundary
+from boundary_class import Boundary
+from functions import PercentChance
 
 class person_obj:
     
     def __init__(self, x, y, vx, vy, status):
         
         # Attributes of each person
         self.x = x                  # Cartisan location
```

## ajm1102pandemic2d/simulation_class.py

```diff
@@ -1,25 +1,17 @@
-import pandas as pd
-import numpy as np
-import matplotlib.pyplot as plt
-import json
-from matplotlib.animation import FuncAnimation
-import random
+
 
 from virus_class import virus
 from person_class import person_obj
-from boundary_class import virus
-
-def randomint(start, end):
-    return np.random.randint(start, end)
-def PercentChance(percent):
-    return random.uniform(0,100) < percent
-
-def Sort2(sub_li):
-    return(sorted(sub_li, key = lambda x: str(x)))  
+from boundary_class import Boundary
+from functions import *
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from matplotlib.animation import FuncAnimation
 
 class simulation:
 
     def __init__(self, sim_length, initial_infectors, num_people):
 
         self.sim_length = sim_length
         self.initial_infectors = initial_infectors
```


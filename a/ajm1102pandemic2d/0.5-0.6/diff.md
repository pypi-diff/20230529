# Comparing `tmp/ajm1102pandemic2d-0.5-py3-none-any.whl.zip` & `tmp/ajm1102pandemic2d-0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 7577 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat       45 b- defN 23-May-29 19:48 ajm1102pandemic2d/__init__.py
+Zip file size: 7830 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      103 b- defN 23-May-29 19:57 ajm1102pandemic2d/__init__.py
 -rw-rw-rw-  2.0 fat       41 b- defN 23-May-29 19:35 ajm1102pandemic2d/boundary_class.py
 -rw-rw-rw-  2.0 fat      254 b- defN 23-May-29 19:45 ajm1102pandemic2d/functions.py
--rw-rw-rw-  2.0 fat     2528 b- defN 23-May-29 19:44 ajm1102pandemic2d/person_class.py
+-rw-rw-rw-  2.0 fat     2582 b- defN 23-May-29 19:56 ajm1102pandemic2d/person_class.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-29 19:53 ajm1102pandemic2d/run.py
 -rw-rw-rw-  2.0 fat     7453 b- defN 23-May-29 18:59 ajm1102pandemic2d/simulation.py
--rw-rw-rw-  2.0 fat     7234 b- defN 23-May-29 19:46 ajm1102pandemic2d/simulation_class.py
+-rw-rw-rw-  2.0 fat     7306 b- defN 23-May-29 19:56 ajm1102pandemic2d/simulation_class.py
 -rw-rw-rw-  2.0 fat       89 b- defN 23-May-29 18:59 ajm1102pandemic2d/virus_class.py
--rw-rw-rw-  2.0 fat      288 b- defN 23-May-29 19:49 ajm1102pandemic2d-0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 19:49 ajm1102pandemic2d-0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-May-29 19:49 ajm1102pandemic2d-0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      948 b- defN 23-May-29 19:49 ajm1102pandemic2d-0.5.dist-info/RECORD
-11 files, 18990 bytes uncompressed, 5945 bytes compressed:  68.7%
+-rw-rw-rw-  2.0 fat      288 b- defN 23-May-29 19:59 ajm1102pandemic2d-0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 19:59 ajm1102pandemic2d-0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-29 19:59 ajm1102pandemic2d-0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1027 b- defN 23-May-29 19:59 ajm1102pandemic2d-0.6.dist-info/RECORD
+12 files, 19253 bytes uncompressed, 6074 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -6,29 +6,32 @@
 
 Filename: ajm1102pandemic2d/functions.py
 Comment: 
 
 Filename: ajm1102pandemic2d/person_class.py
 Comment: 
 
+Filename: ajm1102pandemic2d/run.py
+Comment: 
+
 Filename: ajm1102pandemic2d/simulation.py
 Comment: 
 
 Filename: ajm1102pandemic2d/simulation_class.py
 Comment: 
 
 Filename: ajm1102pandemic2d/virus_class.py
 Comment: 
 
-Filename: ajm1102pandemic2d-0.5.dist-info/METADATA
+Filename: ajm1102pandemic2d-0.6.dist-info/METADATA
 Comment: 
 
-Filename: ajm1102pandemic2d-0.5.dist-info/WHEEL
+Filename: ajm1102pandemic2d-0.6.dist-info/WHEEL
 Comment: 
 
-Filename: ajm1102pandemic2d-0.5.dist-info/top_level.txt
+Filename: ajm1102pandemic2d-0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: ajm1102pandemic2d-0.5.dist-info/RECORD
+Filename: ajm1102pandemic2d-0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ajm1102pandemic2d/__init__.py

```diff
@@ -1,3 +1,4 @@
 
 
-from simulation_class import simulation
+from ajm1102pandemic2d.simulation_class import simulation
+simulation(100,4,4).generate_animation()
```

## ajm1102pandemic2d/person_class.py

```diff
@@ -1,11 +1,11 @@
 import numpy as np
-from virus_class import virus
-from boundary_class import Boundary
-from functions import PercentChance
+from ajm1102pandemic2d.virus_class import virus
+from ajm1102pandemic2d.boundary_class import Boundary
+from ajm1102pandemic2d.functions import PercentChance
 
 class person_obj:
     
     def __init__(self, x, y, vx, vy, status):
         
         # Attributes of each person
         self.x = x                  # Cartisan location
```

## ajm1102pandemic2d/simulation_class.py

```diff
@@ -1,13 +1,13 @@
 
 
-from virus_class import virus
-from person_class import person_obj
-from boundary_class import Boundary
-from functions import *
+from ajm1102pandemic2d.virus_class import virus
+from ajm1102pandemic2d.person_class import person_obj
+from ajm1102pandemic2d.boundary_class import Boundary
+from ajm1102pandemic2d.functions import *
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation
 
 class simulation:
```

## Comparing `ajm1102pandemic2d-0.5.dist-info/RECORD` & `ajm1102pandemic2d-0.6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-ajm1102pandemic2d/__init__.py,sha256=Fq9Jof82E5NBvlBFS9slywHegLCU9hBGqyrvD_cYP0s,45
+ajm1102pandemic2d/__init__.py,sha256=DoJsgiC5LnN9HyG0BgP3KsxF1_LUfmGgVpIktRAo7fY,103
 ajm1102pandemic2d/boundary_class.py,sha256=l80HX2L6N6JV9Md8TfBMh3Za67IuzOJd0LrmcbfLCn4,41
 ajm1102pandemic2d/functions.py,sha256=XumtJHjJdM2s_JQuDaAFyK_mG4UUvfWmEP43uwgycWo,254
-ajm1102pandemic2d/person_class.py,sha256=Z2kY_1L_DhLBrYrdFSO4w5sWj50FeZHRD295wKVqdPM,2528
+ajm1102pandemic2d/person_class.py,sha256=svCPOfdvP47gjkXAogxIJC44YbBIn3UIhWr8rzq04Y0,2582
+ajm1102pandemic2d/run.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ajm1102pandemic2d/simulation.py,sha256=YXrnErWjo6OcJsuANdVqExtH1XVN8sgLZEVGZPfj9Qo,7453
-ajm1102pandemic2d/simulation_class.py,sha256=nTkw0d9lMCSKFlJpoGaFMq0qQVb_1vyDoDiZ8DfQuJw,7234
+ajm1102pandemic2d/simulation_class.py,sha256=Qe-gIZ99EgiRQo9pPtMWwykim9p5SSZq2VYAEdudSDk,7306
 ajm1102pandemic2d/virus_class.py,sha256=As7sO_UmR3Qmxem_iN2KfDNoRfPzmLd48-jI3XIilvY,89
-ajm1102pandemic2d-0.5.dist-info/METADATA,sha256=DxFHrlGF8ACHzREhVFo7cuWog_sTByQ6LyFVkJrYmlU,288
-ajm1102pandemic2d-0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ajm1102pandemic2d-0.5.dist-info/top_level.txt,sha256=dbfceC_sctK0vAYrIzSWVbe0sDDJvnEH6I6n4F6tCrc,18
-ajm1102pandemic2d-0.5.dist-info/RECORD,,
+ajm1102pandemic2d-0.6.dist-info/METADATA,sha256=yfmuEQMAT6W1TpBVcPwmkdAGzKhyTKVaOSIJ5GZkD0c,288
+ajm1102pandemic2d-0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+ajm1102pandemic2d-0.6.dist-info/top_level.txt,sha256=dbfceC_sctK0vAYrIzSWVbe0sDDJvnEH6I6n4F6tCrc,18
+ajm1102pandemic2d-0.6.dist-info/RECORD,,
```


# Comparing `tmp/mrmr_selection-0.2.6-py3-none-any.whl.zip` & `tmp/mrmr_selection-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 24775 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      170 b- defN 23-Feb-18 21:59 mrmr/__init__.py
+Zip file size: 15089 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      185 b- defN 23-May-29 21:01 mrmr/__init__.py
 -rw-rw-rw-  2.0 fat    12053 b- defN 22-Feb-18 21:49 mrmr/bigquery.py
 -rw-rw-rw-  2.0 fat     5755 b- defN 22-Feb-18 21:29 mrmr/main.py
 -rw-rw-rw-  2.0 fat    11095 b- defN 22-Apr-23 18:25 mrmr/pandas.py
+-rw-rw-rw-  2.0 fat     8613 b- defN 23-May-28 22:00 mrmr/polars.py
 -rw-rw-rw-  2.0 fat     8402 b- defN 22-Feb-19 16:57 mrmr/spark.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Feb-18 22:11 mrmr_selection-0.2.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6024 b- defN 23-Feb-18 22:11 mrmr_selection-0.2.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-18 22:11 mrmr_selection-0.2.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Feb-18 22:11 mrmr_selection-0.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      778 b- defN 23-Feb-18 22:11 mrmr_selection-0.2.6.dist-info/RECORD
-10 files, 80197 bytes uncompressed, 23463 bytes compressed:  70.7%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-29 21:12 mrmr_selection-0.2.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6024 b- defN 23-May-29 21:12 mrmr_selection-0.2.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 21:12 mrmr_selection-0.2.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-29 21:12 mrmr_selection-0.2.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      848 b- defN 23-May-29 21:12 mrmr_selection-0.2.7.dist-info/RECORD
+11 files, 54159 bytes uncompressed, 13673 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -6,26 +6,29 @@
 
 Filename: mrmr/main.py
 Comment: 
 
 Filename: mrmr/pandas.py
 Comment: 
 
+Filename: mrmr/polars.py
+Comment: 
+
 Filename: mrmr/spark.py
 Comment: 
 
-Filename: mrmr_selection-0.2.6.dist-info/LICENSE
+Filename: mrmr_selection-0.2.7.dist-info/LICENSE
 Comment: 
 
-Filename: mrmr_selection-0.2.6.dist-info/METADATA
+Filename: mrmr_selection-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: mrmr_selection-0.2.6.dist-info/WHEEL
+Filename: mrmr_selection-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: mrmr_selection-0.2.6.dist-info/top_level.txt
+Filename: mrmr_selection-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mrmr_selection-0.2.6.dist-info/RECORD
+Filename: mrmr_selection-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mrmr/__init__.py

```diff
@@ -1,7 +1,8 @@
-from . import bigquery
-from . import pandas
-from . import spark
-from .pandas import mrmr_classif, mrmr_regression
-from .main import mrmr_base
-
-__version__ = "0.2.6"
+from . import bigquery
+from . import pandas
+from . import polars
+from . import spark
+from .pandas import mrmr_classif, mrmr_regression
+from .main import mrmr_base
+
+__version__ = "0.2.7"
```

## Comparing `mrmr_selection-0.2.6.dist-info/METADATA` & `mrmr_selection-0.2.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrmr-selection
-Version: 0.2.6
+Version: 0.2.7
 Summary: minimum-Redundancy-Maximum-Relevance algorithm for feature selection
 Home-page: https://github.com/smazzanti/mrmr
 Author: Samuele Mazzanti
 Author-email: mazzanti.sam@gmail.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `mrmr_selection-0.2.6.dist-info/RECORD` & `mrmr_selection-0.2.7.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-mrmr/__init__.py,sha256=3iEPECqoQWxSSdlY7HtDCNq2FlapB9Q9WqWm4ebkeSU,170
+mrmr/__init__.py,sha256=Yza9tSaKGqyN1IRJLwo36OFW4MPh7IPcPA--PA_i_nA,185
 mrmr/bigquery.py,sha256=chrRFmUOKZsDQK0JEbtrlMwuLjRgJrtJF6obCtocEYo,12053
 mrmr/main.py,sha256=X7UWDLL_2cHUEdRc-XBxm4MZ52cS6JkFViz28nPLBnU,5755
 mrmr/pandas.py,sha256=Gba1oM0-Tenc5mLODj8ZXUwtNVOVbUsl9nRqbJohbyI,11095
+mrmr/polars.py,sha256=oK_NkJazZI7wtSySIBR3aE7TJXK3Oplab9GywX3Ok9g,8613
 mrmr/spark.py,sha256=pV3McNR4EhdKO2G_mj3zVEdJBEJS1C2MQA7q-Wu2xnY,8402
-mrmr_selection-0.2.6.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-mrmr_selection-0.2.6.dist-info/METADATA,sha256=nPocJLc7OqejxWzjV1Y102h7ndsYtcQTyn1XL1OTuuA,6024
-mrmr_selection-0.2.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-mrmr_selection-0.2.6.dist-info/top_level.txt,sha256=MP2YOpJaF61vuzbsuRUuCx1BhAl_Hkry4HW3VgpFTRU,5
-mrmr_selection-0.2.6.dist-info/RECORD,,
+mrmr_selection-0.2.7.dist-info/LICENSE,sha256=GTpLEzZh69N9ehGDEPxJrqXmSYhJ1BxZeTUAQ6HBuE8,1087
+mrmr_selection-0.2.7.dist-info/METADATA,sha256=Lu-ELw1yUR4U7uc5O4N6G1TvyyZ_W4BA-nrXaeTUu_g,6024
+mrmr_selection-0.2.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mrmr_selection-0.2.7.dist-info/top_level.txt,sha256=MP2YOpJaF61vuzbsuRUuCx1BhAl_Hkry4HW3VgpFTRU,5
+mrmr_selection-0.2.7.dist-info/RECORD,,
```


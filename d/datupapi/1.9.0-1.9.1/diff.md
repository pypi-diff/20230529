# Comparing `tmp/datupapi-1.9.0-py3-none-any.whl.zip` & `tmp/datupapi-1.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 58823 bytes, number of entries: 32
+Zip file size: 58830 bytes, number of entries: 32
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jan-20 21:11 datupapi/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jan-20 21:11 datupapi/configure/__init__.py
 -rw-rw-r--  2.0 unx     5750 b- defN 22-Jan-20 21:11 datupapi/configure/config.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jan-20 21:11 datupapi/evaluate/__init__.py
 -rw-rw-r--  2.0 unx     6933 b- defN 22-Jan-20 21:11 datupapi/evaluate/errors.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jan-20 21:11 datupapi/extract/__init__.py
 -rw-r--r--  2.0 unx    53650 b- defN 22-Jan-26 16:27 datupapi/extract/io.py
@@ -23,12 +23,12 @@
 -rw-r--r--  2.0 unx    19404 b- defN 22-Feb-03 14:50 datupapi/training/tft.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jan-20 21:11 datupapi/transform/__init__.py
 -rw-r--r--  2.0 unx    16924 b- defN 22-Feb-03 14:50 datupapi/transform/backtesting.py
 -rw-rw-r--  2.0 unx    45527 b- defN 22-Jan-31 21:34 datupapi/transform/forecasting.py
 -rw-rw-r--  2.0 unx     7813 b- defN 22-Jan-20 21:11 datupapi/transform/ranking.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jan-20 21:11 datupapi/utils/__init__.py
 -rw-rw-r--  2.0 unx     4637 b- defN 22-Jan-20 21:11 datupapi/utils/utils.py
--rw-rw-r--  2.0 unx      980 b- defN 22-Feb-03 14:53 datupapi-1.9.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Feb-03 14:53 datupapi-1.9.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 22-Feb-03 14:53 datupapi-1.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2643 b- defN 22-Feb-03 14:53 datupapi-1.9.0.dist-info/RECORD
-32 files, 306808 bytes uncompressed, 54563 bytes compressed:  82.2%
+-rw-rw-r--  2.0 unx     1011 b- defN 22-Feb-03 17:32 datupapi-1.9.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Feb-03 17:32 datupapi-1.9.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 22-Feb-03 17:32 datupapi-1.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2644 b- defN 22-Feb-03 17:32 datupapi-1.9.1.dist-info/RECORD
+32 files, 306840 bytes uncompressed, 54570 bytes compressed:  82.2%
```

## zipnote {}

```diff
@@ -78,20 +78,20 @@
 
 Filename: datupapi/utils/__init__.py
 Comment: 
 
 Filename: datupapi/utils/utils.py
 Comment: 
 
-Filename: datupapi-1.9.0.dist-info/METADATA
+Filename: datupapi-1.9.1.dist-info/METADATA
 Comment: 
 
-Filename: datupapi-1.9.0.dist-info/WHEEL
+Filename: datupapi-1.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: datupapi-1.9.0.dist-info/top_level.txt
+Filename: datupapi-1.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: datupapi-1.9.0.dist-info/RECORD
+Filename: datupapi-1.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `datupapi-1.9.0.dist-info/METADATA` & `datupapi-1.9.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.9.0
+Version: 1.9.1
 Summary: Utility library to support Datup AI/MLOps processes
 Home-page: UNKNOWN
 Author: Ramiro Chaparro-Vargas
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Dist: beautifulsoup4 (>=4.9.3)
 Requires-Dist: boto3 (>=1.16.54)
+Requires-Dist: catboost (>=1.0.4)
 Requires-Dist: datetime (>=4.3)
 Requires-Dist: dowhy (>=0.6)
 Requires-Dist: mysql-connector-python (>=8.0.24)
 Requires-Dist: openpyxl (>=3.0.6)
 Requires-Dist: pandas (>=1.3.4)
 Requires-Dist: pymysql (>=1.0.2)
 Requires-Dist: pytest (>=6.2.1)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: pyyaml (>=5.3.1)
 Requires-Dist: requests (>=2.25.1)
 Requires-Dist: scikit-learn (>=0.24.1)
+Requires-Dist: shap (>=0.40.0)
 Requires-Dist: snowflake-connector-python[pandas] (>=2.5.0)
 Requires-Dist: snowflake-sqlalchemy (>=1.3.1)
 Requires-Dist: SQLAlchemy (>=1.3.22)
 Requires-Dist: tensorflow (>=2.6.0)
 Requires-Dist: unidecode (>=1.1.2)
+Requires-Dist: xgboost (>=1.5.2)
 Requires-Dist: xlrd (>=1.0.0)
-Requires-Dist: shap
-Requires-Dist: xgboost
-Requires-Dist: catboost
 
 UNKNOWN
```

## Comparing `datupapi-1.9.0.dist-info/RECORD` & `datupapi-1.9.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 datupapi/training/tft.py,sha256=S99NnmrnTLeTHsodw1p3gnghwsbk6KymrckQF17V-NQ,19404
 datupapi/transform/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 datupapi/transform/backtesting.py,sha256=Hku4n2iuNiGdfusw7ihufzSa1r7T5v_1WoLV_91h7ag,16924
 datupapi/transform/forecasting.py,sha256=fRWMXlFjlpS88quVfZF4N_g3qIW_ZposDtRUxfAsvBU,45527
 datupapi/transform/ranking.py,sha256=5tXSiQ7QfuCLDpI1KgbBQaS7-qOPM7XrARA0B2WzMJw,7813
 datupapi/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 datupapi/utils/utils.py,sha256=pU3mXPupm-1gvODI-kPlIpOdMHa2F9lEXvqBn6t3ajc,4637
-datupapi-1.9.0.dist-info/METADATA,sha256=4IUbOa8AB6vHCdCFj5LtISnS-hfzD9SWCu0eb1q24uU,980
-datupapi-1.9.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-datupapi-1.9.0.dist-info/top_level.txt,sha256=oERwtRZu8xq2u1TDGwJwuWK0iJbH4p7x9kYECAL5So0,9
-datupapi-1.9.0.dist-info/RECORD,,
+datupapi-1.9.1.dist-info/METADATA,sha256=UqAFaBiOVqhDUF8D-RZ5QLIcB_QKB3CmxDx0_4E4w7Y,1011
+datupapi-1.9.1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+datupapi-1.9.1.dist-info/top_level.txt,sha256=oERwtRZu8xq2u1TDGwJwuWK0iJbH4p7x9kYECAL5So0,9
+datupapi-1.9.1.dist-info/RECORD,,
```


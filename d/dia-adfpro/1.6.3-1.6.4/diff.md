# Comparing `tmp/dia-adfpro-1.6.3.tar.gz` & `tmp/dia-adfpro-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dia-adfpro-1.6.3.tar", last modified: Thu May 18 07:37:14 2023, max compression
+gzip compressed data, was "dia-adfpro-1.6.4.tar", last modified: Mon May 29 15:06:50 2023, max compression
```

## Comparing `dia-adfpro-1.6.3.tar` & `dia-adfpro-1.6.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 07:37:14.900493 dia-adfpro-1.6.3/
--rw-rw-rw-   0        0        0     1089 2023-05-18 07:27:08.000000 dia-adfpro-1.6.3/LICENSE.txt
--rw-rw-rw-   0        0        0       17 2023-05-18 07:27:08.000000 dia-adfpro-1.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1069 2023-05-18 07:37:14.900493 dia-adfpro-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      685 2021-02-11 11:49:55.000000 dia-adfpro-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 07:37:14.545089 dia-adfpro-1.6.3/dia_adfpro.egg-info/
--rw-rw-rw-   0        0        0     1069 2023-05-18 07:37:14.000000 dia-adfpro-1.6.3/dia_adfpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-05-18 07:37:14.000000 dia-adfpro-1.6.3/dia_adfpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 07:37:14.000000 dia-adfpro-1.6.3/dia_adfpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 07:37:14.000000 dia-adfpro-1.6.3/dia_adfpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-18 07:37:14.000000 dia-adfpro-1.6.3/dia_adfpro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 07:37:14.545089 dia-adfpro-1.6.3/diaadfpro/
--rw-rw-rw-   0        0        0      295 2023-05-18 07:36:52.000000 dia-adfpro-1.6.3/diaadfpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:37:14.730237 dia-adfpro-1.6.3/diaadfpro/adfpro/
--rw-rw-rw-   0        0        0      270 2022-08-01 06:46:08.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/__init__.py
--rw-rw-rw-   0        0        0    10059 2023-05-18 07:27:08.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/classify.py
--rw-rw-rw-   0        0        0    13958 2023-04-05 13:22:26.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/configuration.py
--rw-rw-rw-   0        0        0     3268 2022-10-24 07:17:27.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/constants.py
--rw-rw-rw-   0        0        0     1334 2022-08-01 06:46:08.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/explain.py
--rw-rw-rw-   0        0        0    28660 2023-05-18 07:36:38.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/feature_extract.py
--rw-rw-rw-   0        0        0    16597 2023-03-27 10:16:17.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/feature_extractors.py
--rw-rw-rw-   0        0        0    10096 2022-08-01 06:46:08.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/golden.py
--rw-rw-rw-   0        0        0    14313 2023-04-28 12:40:42.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/model.py
--rw-rw-rw-   0        0        0     7455 2022-10-24 07:17:27.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/offload.py
--rw-rw-rw-   0        0        0     7607 2023-04-28 12:40:42.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/train.py
--rw-rw-rw-   0        0        0    54884 2023-05-18 07:27:08.000000 dia-adfpro-1.6.3/diaadfpro/adfpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:37:14.900493 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/
--rw-rw-rw-   0        0        0      268 2022-08-01 06:46:08.000000 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/__init__.py
--rw-rw-rw-   0        0        0     4014 2023-05-18 07:36:52.000000 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/constants.py
--rw-rw-rw-   0        0        0     6149 2022-08-02 08:08:38.000000 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_anomaly_plots.py
--rw-rw-rw-   0        0        0    11741 2022-10-24 07:17:27.000000 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_app.py
--rw-rw-rw-   0        0        0    20412 2022-10-24 07:17:27.000000 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_components.py
--rw-rw-rw-   0        0        0     1167 2021-09-23 15:24:24.000000 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_env_cfg.py
--rw-rw-rw-   0        0        0     1243 2022-08-01 06:46:08.000000 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_env_cfg.sample.py
--rw-rw-rw-   0        0        0     3677 2022-08-02 08:08:38.000000 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_ohlc_plots.py
--rw-rw-rw-   0        0        0     6925 2022-10-24 07:17:27.000000 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_retrain.py
--rw-rw-rw-   0        0        0    10252 2022-08-02 08:08:38.000000 dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_summary_table.py
--rw-rw-rw-   0        0        0      115 2023-05-18 07:37:14.900493 dia-adfpro-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1239 2023-05-18 07:27:08.000000 dia-adfpro-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:49.993913 dia-adfpro-1.6.4/
+-rw-rw-rw-   0        0        0     1089 2023-05-18 08:28:18.000000 dia-adfpro-1.6.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       17 2023-05-18 08:28:18.000000 dia-adfpro-1.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1046 2023-05-29 15:06:49.994913 dia-adfpro-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2021-02-11 11:49:55.000000 dia-adfpro-1.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:49.639890 dia-adfpro-1.6.4/dia_adfpro.egg-info/
+-rw-rw-rw-   0        0        0     1046 2023-05-29 15:06:49.000000 dia-adfpro-1.6.4/dia_adfpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2023-05-29 15:06:49.000000 dia-adfpro-1.6.4/dia_adfpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 15:06:49.000000 dia-adfpro-1.6.4/dia_adfpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 15:06:49.000000 dia-adfpro-1.6.4/dia_adfpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-29 15:06:49.000000 dia-adfpro-1.6.4/dia_adfpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:49.643886 dia-adfpro-1.6.4/diaadfpro/
+-rw-rw-rw-   0        0        0      295 2023-05-29 15:06:01.000000 dia-adfpro-1.6.4/diaadfpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:49.841902 dia-adfpro-1.6.4/diaadfpro/adfpro/
+-rw-rw-rw-   0        0        0      270 2022-08-01 06:46:08.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/__init__.py
+-rw-rw-rw-   0        0        0    10059 2023-05-18 08:28:18.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/classify.py
+-rw-rw-rw-   0        0        0    13958 2023-05-26 14:18:50.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/configuration.py
+-rw-rw-rw-   0        0        0     3268 2022-10-24 07:17:27.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/constants.py
+-rw-rw-rw-   0        0        0     1334 2022-08-01 06:46:08.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/explain.py
+-rw-rw-rw-   0        0        0    31018 2023-05-29 15:05:41.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/feature_extract.py
+-rw-rw-rw-   0        0        0    16597 2023-03-27 10:16:17.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/feature_extractors.py
+-rw-rw-rw-   0        0        0    10096 2022-08-01 06:46:08.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/golden.py
+-rw-rw-rw-   0        0        0    14313 2023-04-28 12:40:42.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/model.py
+-rw-rw-rw-   0        0        0     7455 2022-10-24 07:17:27.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/offload.py
+-rw-rw-rw-   0        0        0     7607 2023-04-28 12:40:42.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/train.py
+-rw-rw-rw-   0        0        0    54884 2023-05-18 08:28:18.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:06:49.991914 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/
+-rw-rw-rw-   0        0        0      268 2022-08-01 06:46:08.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/__init__.py
+-rw-rw-rw-   0        0        0     4014 2023-05-29 15:06:01.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/constants.py
+-rw-rw-rw-   0        0        0     6149 2022-08-02 08:08:38.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_anomaly_plots.py
+-rw-rw-rw-   0        0        0    11741 2022-10-24 07:17:27.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_app.py
+-rw-rw-rw-   0        0        0    20412 2022-10-24 07:17:27.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_components.py
+-rw-rw-rw-   0        0        0     1167 2021-09-23 15:24:24.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_env_cfg.py
+-rw-rw-rw-   0        0        0     1243 2022-08-01 06:46:08.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_env_cfg.sample.py
+-rw-rw-rw-   0        0        0     3677 2022-08-02 08:08:38.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_ohlc_plots.py
+-rw-rw-rw-   0        0        0     6925 2022-10-24 07:17:27.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_retrain.py
+-rw-rw-rw-   0        0        0    10252 2022-08-02 08:08:38.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_summary_table.py
+-rw-rw-rw-   0        0        0      115 2023-05-29 15:06:49.996911 dia-adfpro-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1239 2023-05-18 08:28:18.000000 dia-adfpro-1.6.4/setup.py
```

### Comparing `dia-adfpro-1.6.3/LICENSE.txt` & `dia-adfpro-1.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/PKG-INFO` & `dia-adfpro-1.6.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: dia-adfpro
-Version: 1.6.3
+Version: 1.6.4
 Summary: A Python application for anomaly detection
 Home-page: https://github.com/EliLillyCo/MQIT_DIA_ADFPRO
 Author: Francesco Gabbanini, Manjunath Bagewadi, Henson Tauro
 Author-email: fgabbanini@yahoo.it
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MQIT_DIA_ADFPRO
 Anomaly Detection for Fast PROcesses (ADFPRO) is a Python application used to implement anomaly detection for "fast" processes that can be described by multiple features.
 Fast means processes that are repeated continuously on manufacturing equipments and have a duration of a few seconds.
 
 Repository includes 2 modules:
 1) used from ML frameworks running on the cloud (Domino, SageMaker, AzureML) to trigger model training and classification on datasets having a certain structure;
 2) used to implement Dash dashboards to visualize results
 
 Uses code contained in MQIT_DIA_AIML_Toolkit.
 
 Developed and maintained by MQ-IDS Data Integration and Analytics.
-
-
```

### Comparing `dia-adfpro-1.6.3/README.md` & `dia-adfpro-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/dia_adfpro.egg-info/PKG-INFO` & `dia-adfpro-1.6.4/dia_adfpro.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: dia-adfpro
-Version: 1.6.3
+Version: 1.6.4
 Summary: A Python application for anomaly detection
 Home-page: https://github.com/EliLillyCo/MQIT_DIA_ADFPRO
 Author: Francesco Gabbanini, Manjunath Bagewadi, Henson Tauro
 Author-email: fgabbanini@yahoo.it
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MQIT_DIA_ADFPRO
 Anomaly Detection for Fast PROcesses (ADFPRO) is a Python application used to implement anomaly detection for "fast" processes that can be described by multiple features.
 Fast means processes that are repeated continuously on manufacturing equipments and have a duration of a few seconds.
 
 Repository includes 2 modules:
 1) used from ML frameworks running on the cloud (Domino, SageMaker, AzureML) to trigger model training and classification on datasets having a certain structure;
 2) used to implement Dash dashboards to visualize results
 
 Uses code contained in MQIT_DIA_AIML_Toolkit.
 
 Developed and maintained by MQ-IDS Data Integration and Analytics.
-
-
```

### Comparing `dia-adfpro-1.6.3/dia_adfpro.egg-info/SOURCES.txt` & `dia-adfpro-1.6.4/dia_adfpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/classify.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/classify.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/configuration.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/configuration.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/constants.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/constants.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/explain.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/explain.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/feature_extract.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/feature_extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import pathlib
 import sys
 import time
 from datetime import datetime, timedelta
 from enum import Enum
 import warnings
+from collections import Counter
 
 import numpy as np
 import pandas as pd
 import pytz
 import copy
 from tqdm import tqdm
 from tzlocal import get_localzone  # $ pip install tzlocal
@@ -27,14 +28,29 @@
 from diaadfpro.adfpro.utils import YMLConfigReader, IOUtils, ADFPDateUtils
 
 logger = logging.getLogger(__name__)
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 DEFAULT_TS_FORMAT = 'YYYY-MM-DD hh:mm:ss+hh:mm'
 
+class FeatureExtractExitCodes(Enum):
+    NO_ERRORS = 0
+    TAG_VALUE_MISMATCH = 1
+    ERR_INVALID_CYCLE_IDENTIFICATION_MODE = 2
+    ERR_DATA_PREPARATION = 3
+    NO_CYCLES_CONTAINING_TAG_VALUES = 4
+    ERR_FEATURE_EXTRACTION = 5
+    ERR_WRITE_FEATURES = 6
+    ERR_TIME_FORMAT = 7
+    ERR_INVALID_FEATURE_CALCULATION_MODE = 8
+    EMPTY_CAPSULE_LIST = 9
+    EMPTY_TAGVALUE_LIST = 10
+    EMPTY_FEATURE_DF = 11
+    UNSPECIFIED_ERROR = 1000
+
 @dataclass
 class FeatureExtractionResults:
     df: pd.DataFrame
     invalid_cycle_cnt: int
     neg_feat_cycle_cnt: int
     zero_feat_cycle_cnt: int
     total_cycle_cnt: int
@@ -193,15 +209,15 @@
             return None
 
     def two_tag_feature_extractor(self, df, tag_list, feat_names, keep_negatives=False, keep_zero=False):
 
         try:
             df_clean_4val = self.__purge_invalid_cycles(df, 4)
         except AssertionError:
-            logger.warning("Percentage of cycles with an invalid number of values ({}) exceeds {}".format(4, self.__invalid_cycles_thr_seg))
+            logger.error("Percentage of cycles with an invalid number of values ({}) exceeds {}".format(4, self.__invalid_cycles_thr_seg))
             return None
         except Exception as e:
             logger.error("Error eliminating cycles with an invalid number of values")
             logger.error("Details: {}".format(e))
             return None
 
         logger.info("Cycles after purging invalid ones: {}".format(len(df_clean_4val.cycle.unique())))
@@ -216,15 +232,15 @@
             return None
 
     def three_tag_feature_extractor(self, df, tag_list, feat_names, keep_negatives=False, keep_zero=False):
 
         try:
             df_clean_4val = self.__purge_invalid_cycles(df, 6)
         except AssertionError:
-            logger.warning("Percentage of cycles with an invalid number of values ({}) exceeds {}".format(6, self.__invalid_cycles_thr_seg))
+            logger.error("Percentage of cycles with an invalid number of values ({}) exceeds {}".format(6, self.__invalid_cycles_thr_seg))
             return None
         except Exception as e:
             logger.error("Error eliminating cycles with an invalid number of values")
             logger.error("Details: {}".format(e))
             return None
 
         logger.info("Cycles after purging invalid ones: {}".format(len(df_clean_4val.cycle.unique())))
@@ -240,15 +256,15 @@
             logger.error("Details: {}".format(e))
             return None
         
     def four_tag_feature_extractor(self, df, tag_list, feat_names, keep_negatives=False, keep_zero=False):
         try:
             df_clean_8val = self.__purge_invalid_cycles(df, 8)
         except AssertionError:
-            logger.warning("Percentage of cycles with an invalid number of values ({}) exceeds {}".format(8, self.__invalid_cycles_thr_seg))
+            logger.error("Percentage of cycles with an invalid number of values ({}) exceeds {}".format(8, self.__invalid_cycles_thr_seg))
             return None
         except Exception as e:
             logger.error("Error eliminating cycles with an invalid number of values")
             logger.error("Details: {}".format(e))
             return None
 
         logger.info("Cycles after purging invalid ones: {}".format(len(df_clean_8val.cycle.unique())))
@@ -332,23 +348,14 @@
 def get_data(pife: PIFeatureExtractor, start_ts, end_ts, max_ti_len_hrs, tag_list, data_path = None, df_data = None):
     try:
         if data_path:
             # filter out data read from local parquet file...
             df = df_data[(df_data.time > str(start_ts)) & (df_data.time < str(end_ts))]
             logger.info("Read from local file ({}). Extracted {} tag values.".format(data_path, len(df)))
         else:
-            # read from PI...but check length of time interval first
-            diff = end_ts - start_ts
-            if diff.total_seconds() > max_ti_len_hrs * 3600:
-                start_ts = end_ts - timedelta(hours=max_ti_len_hrs)
-                logger.warning("Time interval duration exceeds limit ({} hrs). Risk of overloading PI server.".format(
-                    max_ti_len_hrs))
-                logger.warning("RE-SETTING INTERVAL START TO {}.".format(str(start_ts)))
-                logger.warning("NEW TIME INTERVAL IS: ({}, {})".format(start_ts, end_ts))
-
             df = pife.read_tag_data(tag_list, str(start_ts), str(end_ts))
             logger.info("Read from PI ({}). Extracted {} tag values.".format(pife.pi_server_url, len(df)))
         return df
     except Exception as e:
         logger.error("Failure while reading {}".format(tag_list))
         logger.error("Details: {}".format(e))
         logger.error("Skipping to the next component")
@@ -424,28 +431,54 @@
             logger.warning("Please note that cycles having negative feature values will be DISCARDED (idea is that this denotes bad segmentation)")
 
         if not fep.keep_zero_feature_vals:
             logger.warning("Please note that cycles having feature values equal to zero will be DISCARDED (idea is that zero features are due to PLC 50ms resolution limit)")
 
         return fep
 
+
+def failed(exit_codes):
+    errs = [FeatureExtractExitCodes.ERR_INVALID_CYCLE_IDENTIFICATION_MODE,
+            FeatureExtractExitCodes.ERR_DATA_PREPARATION,
+            FeatureExtractExitCodes.ERR_FEATURE_EXTRACTION,
+            FeatureExtractExitCodes.ERR_WRITE_FEATURES,
+            FeatureExtractExitCodes.ERR_TIME_FORMAT,
+            FeatureExtractExitCodes.ERR_INVALID_FEATURE_CALCULATION_MODE]
+
+    if len(set(errs).intersection(exit_codes)) > 0:
+        return True
+
+    return False
+
+
+def reset_time_interval_start(start_ts, end_ts, max_ti_len_hrs):
+    new_start_ts = start_ts
+    diff = end_ts - new_start_ts
+    if diff.total_seconds() > max_ti_len_hrs * 3600:
+        new_start_ts = end_ts - timedelta(hours=max_ti_len_hrs)
+        logger.warning("Time interval duration exceeds limit ({} hrs). Risk of overloading PI server.".format(
+            max_ti_len_hrs))
+        logger.warning("RE-SETTING INTERVAL START TO {}.".format(str(start_ts)))
+        logger.warning("NEW TIME INTERVAL IS: ({}, {})".format(start_ts, end_ts))
+    return new_start_ts
+
 def main(argv):
     if len(argv) < 1:
         logger.error("Not enough input arguments")
-        return
+        sys.exit(1)
 
     [cfg_path, data_path] = parse_options(argv)
     logger.info("Using configuration file: {}".format(cfg_path))
 
     cfg_dict = YMLConfigReader.read_full_path(cfg_path)
 
     if not 'log cfg file' in cfg_dict:
         logger.error("Please specify a valid path to a configuration file for the logger")
         logger.error("Use \'{}\' as a key in {}".format('log cfg file', cfg_path))
-        return
+        sys.exit(1)
     else:
         featextract_cfg_log_path = cfg_dict['log cfg file']
         logging.config.fileConfig(featextract_cfg_log_path, disable_existing_loggers=False)
         logger.warning("Using log configuration file at {}".format(featextract_cfg_log_path))
 
     logger.info(">>> Start data extraction and feature calculation <<<")
     logger.info("Using {} from ADFPRO {}".format(__file__, diaadfpro.__version__))
@@ -484,117 +517,141 @@
 
     resolution_millisec = 50
     if 'resolution millisec' in cfg_dict['pi read']:
         resolution_millisec = cfg_dict['pi read']['resolution millisec']
 
     tot_cmp = len(cmp_dict.keys())
     cur_cmp = 0
+    exit_codes = []
     start_calc = time.time()
     for cmp_name in cmp_dict.keys():
         logger.info(f"===Calculating features for component {cmp_name} ({cur_cmp} of {tot_cmp})")
         start_cmp_calc = time.time()
         cur_cmp += 1
         
         fep = FeatureExtractionParameters.build_from_dictionary(cmp_dict[cmp_name])
         logger.info("Tags: {}".format(fep.tags_list))
 
         if not fixed_ti:
             start_ts = cmp_dict[cmp_name]['latest']
             if isinstance(start_ts, str) or (not ADFPDateUtils.is_tz_aware(start_ts)):
+                exit_codes.append(FeatureExtractExitCodes.ERR_TIME_FORMAT)
                 logger.error("Start time should be timezone aware! Please fix it in the 'latest' key of the configuration file, related to the component named {}".format(cmp_name))
                 logger.error("Please use {} as a format".format(DEFAULT_TS_FORMAT))
-                return
+                logger.error("Skipping to the next component")
+                continue
 
         logger.info("Time interval: ({}, {})".format(start_ts, end_ts))
+        start_ts = reset_time_interval_start(start_ts, end_ts, max_ti_len_hrs)
 
         if cycle_identification_mode == 'sequencer':
             data_prep = DataPreparator.build_sequencer_data_preparator(fep.tag_sequencer_name, fep.tags_list, fep.thr_val)
         elif cycle_identification_mode == 'capsules':
             fep.tag_sequencer_name = None
             logger.info(f"Building capsule data preparator. Workbook: {workbook_id}, capsule: {fep.capsule_id}, by name: {read_by_name}")
             df_capsules = pife.read_capsule_data([fep.capsule_id], start_ts, end_ts, workbook_id=workbook_id, by_name=read_by_name)
             if df_capsules is None:
+                # warning already logged in pife.read_capsule_data...no need to log again
+                exit_codes.append(FeatureExtractExitCodes.EMPTY_CAPSULE_LIST)
                 continue
             else:
                 data_prep = DataPreparator.build_capsule_data_preparator(df_capsules, adjust_capsules_for_resolution, resolution_millisec)
         else:
-            logger.error(f"Invalid cycle identification mode {cycle_identification_mode}")
+            exit_codes.append(FeatureExtractExitCodes.ERR_INVALID_CYCLE_IDENTIFICATION_MODE)
+            logger.error(f"Invalid cycle identification mode: {cycle_identification_mode}")
             logger.error("Skipping to the next component")
+            continue
 
         if data_path:
             df = get_data(pife, start_ts, end_ts, max_ti_len_hrs, fep.full_tag_list, data_path, df_data_from_file)
         else:
             df = get_data(pife, start_ts, end_ts, max_ti_len_hrs, fep.full_tag_list)
 
         if len(df) == 0:
+            exit_codes.append(FeatureExtractExitCodes.EMPTY_TAGVALUE_LIST)
             logger.warning("No tag values available in given time interval. Tags: {}, start: {}, end: {}".format(fep.tags_list, start_ts, end_ts))
             continue
 
         try:
             df_clean = data_prep.prepare_data(df)
         except:
+            exit_codes.append(FeatureExtractExitCodes.ERR_DATA_PREPARATION)
             logger.error(f"Unable to run data preparation (cycle segmentation related operations)")
             logger.error("Skipping to the next component")
             continue
 
         if len(df_clean) == 0:
+            exit_codes.append(FeatureExtractExitCodes.NO_CYCLES_CONTAINING_TAG_VALUES)
             logger.error(f"Unable to identify any cycle that contains valid tag values")
             logger.error("Skipping to the next component")
             continue
 
         if fep.feature_calculation_mode == FeatureCalculationMode.SIMPLE_2WISE:
             feat_extr_results = pife.two_tag_feature_extractor(df_clean, fep.tags_list, fep.feats_list, fep.keep_neg_feature_vals, fep.keep_zero_feature_vals)
         elif fep.feature_calculation_mode == FeatureCalculationMode.SIMPLE_3WISE:
             feat_extr_results = pife.three_tag_feature_extractor(df_clean, fep.tags_list, fep.feats_list, fep.keep_neg_feature_vals, fep.keep_zero_feature_vals)
         elif fep.feature_calculation_mode == FeatureCalculationMode.SIMPLE_4WISE:
             feat_extr_results = pife.four_tag_feature_extractor(df_clean, fep.tags_list, fep.feats_list, fep.keep_neg_feature_vals, fep.keep_zero_feature_vals)
         else:
-            logger.warning("Unknown feature calculation mode. Skipping to next component.")
+            exit_codes.append(FeatureExtractExitCodes.ERR_INVALID_FEATURE_CALCULATION_MODE)
+            logger.error("Unknown feature calculation mode. Skipping to next component.")
             continue
 
         if feat_extr_results is None:
-            logger.warning("Error calculating features or empty feature set. Skipping to next component.")
+            exit_codes.append(FeatureExtractExitCodes.ERR_FEATURE_EXTRACTION)
+            logger.error("Error calculating features or empty feature set. Skipping to next component.")
             continue
 
         df_feat = feat_extr_results.df
         if df_feat is None or len(df_feat) == 0:
+            exit_codes.append(FeatureExtractExitCodes.EMPTY_FEATURE_DF)
             logger.warning("Error calculating features or empty feature set. Skipping to next component.")
             continue
             
         logger.info("Calculated {} feature rows".format(len(df_feat)))
 
         # write features to DB and update timestamp on configuration file
         dbp = cfg_dict['DB']
         if dbp[ADFPC.STR_WRITE_ENABLED]:
             try:
                 start = time.time()
-                logger.info("Start writing to DB...")
+                logger.info("Start writing features...")
                 IOUtils.write_features(df_feat, dbp, os.environ[dbp[ADFPC.STR_PWD_ENVVAR]])
                 tsecs = round(time.time()-start, 2)
-                logger.info("Wrote {} rows on DB. Time: {}s (includes query preparation).".format(len(df_feat), tsecs))
+                logger.info("Wrote {} feature rows. Time: {}s (includes query preparation).".format(len(df_feat), tsecs))
                 if not fixed_ti:
                     #save time on yml file
                     cmp_dict[cmp_name]['latest'] = copy.deepcopy(end_ts)
                     YMLConfigReader.write(cfg_dict, cfg_path)
                     logger.info("Updated latest timestamp for successful feature calculation")
             except Exception as e:
-                logger.error("Error while writing to DB or updating timestamp on configuration file")
+                exit_codes.append(FeatureExtractExitCodes.ERR_WRITE_FEATURES)
+                logger.error("Error while writing features or updating timestamp on configuration file")
                 logger.error("Details: {}".format(e))
 
         if 'dump csv' in cfg_dict:
             p = pathlib.Path(cfg_dict['dump csv'], cmp_name + '.csv')
             logger.info("Dump features to csv file ({})".format(str(p)))
             df_feat.to_csv(p)
 
         logger.info("===Component {} completed".format(cmp_name))
         tsecs = round(time.time() - start_cmp_calc, 2)
         logger.info(f"===Time: {tsecs}s (includes writing if enabled).")
     logger.info(">>> Feature calculation completed for all components in configuration file <<<")
+    logger.info(">>> Count of exit codes <<<")
+    logger.info(f">>> Total: {len(exit_codes)}")
+    c = Counter(exit_codes)
+    for n in c.keys():
+        logger.info(f">>> {n}: {c[n]}")
+
     tsecs = round(time.time() - start_calc, 2)
     logger.info(f">>> Time {tsecs}s <<<")
+    if failed(exit_codes):
+        sys.exit(1)
+    sys.exit(0)
 
 if __name__ == "__main__":
     #use -d "C:/Users/c206539/Downloads/M24-STXX.tag.parquet" for reading from local parquet file
     try:
         main(sys.argv[1:])
     except Exception as e:
         logger.error("Failure while running feature extraction")
```

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/feature_extractors.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/golden.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/golden.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/model.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/model.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/offload.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/offload.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/train.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/train.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro/utils.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro/utils.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro_ui/constants.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
             Manjunath C Bagewadi <bagewadi_manjunath_c@lilly.com>, 
             Henson Tauro <tauro_henson@lilly.com> 
             (MQ IDS - Data Integration and Analytics)
 License:    MIT
 """
 
 class ADFPCUI:
-    REPORT_VERSION = "1.6.3 (2023-05-18)"
+    REPORT_VERSION = "1.6.4 (2023-05-29)"
 
     #use for html id's
     ID_REFRESH = "btn-refresh"                                       #Refresh tab1
     ID_LATESTFETCH = "lbl-latestfetch"                               # latestfetch tab1
     ID_SUMMARY_TBL_CONTAINER = "div-summary-tbl-container"
     
     RETRAIN_YML = "/mnt/py/cfg.jobs/temp_retrain_job.yml"
```

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_anomaly_plots.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_anomaly_plots.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_app.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_app.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_components.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_components.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_env_cfg.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_env_cfg.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_env_cfg.sample.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_env_cfg.sample.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_ohlc_plots.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_ohlc_plots.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_retrain.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_retrain.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/diaadfpro/adfpro_ui/ui_summary_table.py` & `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_summary_table.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.3/setup.py` & `dia-adfpro-1.6.4/setup.py`

 * *Files identical despite different names*


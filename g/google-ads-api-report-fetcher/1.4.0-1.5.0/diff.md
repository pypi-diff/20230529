# Comparing `tmp/google-ads-api-report-fetcher-1.4.0.tar.gz` & `tmp/google-ads-api-report-fetcher-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-ads-api-report-fetcher-1.4.0.tar", last modified: Tue May 16 06:26:16 2023, max compression
+gzip compressed data, was "google-ads-api-report-fetcher-1.5.0.tar", last modified: Mon May 29 10:53:28 2023, max compression
```

## Comparing `google-ads-api-report-fetcher-1.4.0.tar` & `google-ads-api-report-fetcher-1.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4222 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3489 2023-03-16 20:20:32.000000 google-ads-api-report-fetcher-1.4.0/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.276760 google-ads-api-report-fetcher-1.4.0/gaarf/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.4.0/gaarf/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7756 2023-04-13 10:50:21.000000 google-ads-api-report-fetcher-1.4.0/gaarf/api_clients.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      916 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.4.0/gaarf/base_query.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3744 2023-04-13 14:02:39.000000 google-ads-api-report-fetcher-1.4.0/gaarf/bq_executor.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.276760 google-ads-api-report-fetcher-1.4.0/gaarf/cli/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.4.0/gaarf/cli/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3671 2023-02-20 08:49:55.000000 google-ads-api-report-fetcher-1.4.0/gaarf/cli/bq.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7841 2023-05-16 06:16:06.000000 google-ads-api-report-fetcher-1.4.0/gaarf/cli/gaarf.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3238 2023-01-30 21:09:38.000000 google-ads-api-report-fetcher-1.4.0/gaarf/cli/simulator.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10557 2023-04-07 06:52:45.000000 google-ads-api-report-fetcher-1.4.0/gaarf/cli/utils.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.276760 google-ads-api-report-fetcher-1.4.0/gaarf/io/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.4.0/gaarf/io/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1842 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.4.0/gaarf/io/formatter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1870 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.4.0/gaarf/io/reader.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9991 2023-03-16 19:54:17.000000 google-ads-api-report-fetcher-1.4.0/gaarf/io/writer.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9666 2023-05-15 07:22:41.000000 google-ads-api-report-fetcher-1.4.0/gaarf/parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9680 2023-03-10 13:35:15.000000 google-ads-api-report-fetcher-1.4.0/gaarf/query_editor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11371 2023-05-04 10:22:26.000000 google-ads-api-report-fetcher-1.4.0/gaarf/query_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5168 2023-05-09 09:54:31.000000 google-ads-api-report-fetcher-1.4.0/gaarf/report.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4088 2023-03-06 16:43:36.000000 google-ads-api-report-fetcher-1.4.0/gaarf/simulation.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2295 2023-05-16 06:16:06.000000 google-ads-api-report-fetcher-1.4.0/gaarf/utils.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      158 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.4.0/gaarf/wip.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4222 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1033 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      120 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/entry_points.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      192 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       12 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       63 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1589 2023-05-16 06:17:39.000000 google-ads-api-report-fetcher-1.4.0/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.4.0/tests/__init__.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/tests/unit/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      748 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_base_query.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1400 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_bq_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10945 2023-04-07 06:54:54.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_cli_utils.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7168 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3890 2023-02-24 15:33:44.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_query_editor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      891 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_reader.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5788 2023-05-11 16:09:08.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_report.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2487 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_simulation.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3864 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_writer.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4222 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3489 2023-03-16 20:20:32.000000 google-ads-api-report-fetcher-1.5.0/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.531231 google-ads-api-report-fetcher-1.5.0/gaarf/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.5.0/gaarf/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7756 2023-04-13 10:50:21.000000 google-ads-api-report-fetcher-1.5.0/gaarf/api_clients.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      916 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.5.0/gaarf/base_query.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3744 2023-05-22 11:14:44.000000 google-ads-api-report-fetcher-1.5.0/gaarf/bq_executor.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/gaarf/cli/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.5.0/gaarf/cli/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4053 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.5.0/gaarf/cli/bq.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     8203 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.5.0/gaarf/cli/gaarf.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3586 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.5.0/gaarf/cli/simulator.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10557 2023-05-18 10:21:29.000000 google-ads-api-report-fetcher-1.5.0/gaarf/cli/utils.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/gaarf/io/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.5.0/gaarf/io/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1842 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.5.0/gaarf/io/formatter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1870 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.5.0/gaarf/io/reader.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     9991 2023-03-16 19:54:17.000000 google-ads-api-report-fetcher-1.5.0/gaarf/io/writer.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10596 2023-05-29 10:48:19.000000 google-ads-api-report-fetcher-1.5.0/gaarf/parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     9680 2023-03-10 13:35:15.000000 google-ads-api-report-fetcher-1.5.0/gaarf/query_editor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11371 2023-05-04 10:22:26.000000 google-ads-api-report-fetcher-1.5.0/gaarf/query_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5655 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.5.0/gaarf/report.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4088 2023-03-06 16:43:36.000000 google-ads-api-report-fetcher-1.5.0/gaarf/simulation.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2295 2023-05-16 06:16:06.000000 google-ads-api-report-fetcher-1.5.0/gaarf/utils.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      158 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.5.0/gaarf/wip.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4222 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1033 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      184 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/entry_points.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      192 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       12 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       63 2023-05-29 10:53:28.539231 google-ads-api-report-fetcher-1.5.0/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1679 2023-05-29 10:48:29.000000 google-ads-api-report-fetcher-1.5.0/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.5.0/tests/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/tests/unit/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      748 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_base_query.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1400 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_bq_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10945 2023-04-07 06:54:54.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_cli_utils.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7168 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3890 2023-02-24 15:33:44.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_query_editor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      891 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_reader.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6927 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_report.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2487 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_simulation.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3864 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_writer.py
```

### Comparing `google-ads-api-report-fetcher-1.4.0/PKG-INFO` & `google-ads-api-report-fetcher-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ads-api-report-fetcher
-Version: 1.4.0
+Version: 1.5.0
 Summary: Library for fetching reports from Google Ads API and saving them locally / BigQuery.
 Home-page: https://github.com/google/ads-api-reports-fetcher
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-ads-api-report-fetcher-1.4.0/README.md` & `google-ads-api-report-fetcher-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/api_clients.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/api_clients.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/base_query.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/base_query.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/bq_executor.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/bq_executor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/cli/bq.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/cli/bq.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
+import sys
 import argparse
 from concurrent import futures
 import logging
 from rich.logging import RichHandler
 
 from gaarf.io import reader  # type: ignore
 from gaarf.bq_executor import BigQueryExecutor
@@ -37,26 +37,34 @@
     parser.add_argument("--no-save-config",
                         dest="save_config",
                         action="store_false")
     parser.add_argument("--config-destination",
                         dest="save_config_dest",
                         default="config.yaml")
     parser.add_argument("--log", "--loglevel", dest="loglevel", default="info")
+    parser.add_argument("--logger", dest="logger", default="local")
     parser.add_argument("--dry-run",
                         dest="dry_run",
                         action="store_true")
     parser.set_defaults(save_config=False)
     parser.set_defaults(dry_run=False)
     args = parser.parse_known_args()
     main_args = args[0]
 
-    logging.basicConfig(format="%(message)s",
-                        level=main_args.loglevel.upper(),
-                        datefmt="%Y-%m-%d %H:%M:%S",
-                        handlers=[RichHandler(rich_tracebacks=True)])
+    if main_args.logger == "rich":
+        logging.basicConfig(format="%(message)s",
+                            level=main_args.loglevel.upper(),
+                            datefmt="%Y-%m-%d %H:%M:%S",
+                            handlers=[RichHandler(rich_tracebacks=True)])
+    else:
+        logging.basicConfig(
+                    format="[%(asctime)s][%(name)s][%(levelname)s] %(message)s",
+                    stream=sys.stdout,
+                    level=main_args.loglevel.upper(),
+                    datefmt="%Y-%m-%d %H:%M:%S")
     logging.getLogger("smart_open.smart_open_lib").setLevel(logging.WARNING)
     logging.getLogger("urllib3.connectionpool").setLevel(logging.WARNING)
     logger = logging.getLogger(__name__)
 
     config = GaarfBqConfigBuilder(args).build()
     logger.debug("config: %s", config)
     if main_args.save_config and not main_args.gaarf_config:
```

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/cli/gaarf.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/cli/gaarf.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any, Dict
-
+import sys
 from collections.abc import MutableSequence
 from concurrent import futures
 import argparse
 from pathlib import Path
 import logging
 from rich.logging import RichHandler
 from smart_open import open
@@ -35,14 +34,15 @@
     parser.add_argument("--output", dest="save", default="console")
     parser.add_argument("--input", dest="input", default="file")
     parser.add_argument("--ads-config",
                         dest="config",
                         default=str(Path.home() / "google-ads.yaml"))
     parser.add_argument("--api-version", dest="api_version", default=12)
     parser.add_argument("--log", "--loglevel", dest="loglevel", default="info")
+    parser.add_argument("--logger", dest="logger", default="local")
     parser.add_argument("--customer-ids-query",
                         dest="customer_ids_query",
                         default=None)
     parser.add_argument("--customer-ids-query-file",
                         dest="customer_ids_query_file",
                         default=None)
     parser.add_argument("--save-config",
@@ -78,18 +78,25 @@
     if main_args.version:
         import pkg_resources
         version = pkg_resources.require(
             "google-ads-api-report-fetcher")[0].version
         print(f"gaarf version {version}")
         exit()
 
-    logging.basicConfig(format="%(message)s",
-                        level=main_args.loglevel.upper(),
-                        datefmt="%Y-%m-%d %H:%M:%S",
-                        handlers=[RichHandler(rich_tracebacks=True)])
+    if main_args.logger == "rich":
+        logging.basicConfig(format="%(message)s",
+                            level=main_args.loglevel.upper(),
+                            datefmt="%Y-%m-%d %H:%M:%S",
+                            handlers=[RichHandler(rich_tracebacks=True)])
+    else:
+        logging.basicConfig(
+                    format="[%(asctime)s][%(name)s][%(levelname)s] %(message)s",
+                    stream=sys.stdout,
+                    level=main_args.loglevel.upper(),
+                    datefmt="%Y-%m-%d %H:%M:%S")
     logging.getLogger("google.ads.googleads.client").setLevel(logging.WARNING)
     logging.getLogger("smart_open.smart_open_lib").setLevel(logging.WARNING)
     logging.getLogger("urllib3.connectionpool").setLevel(logging.WARNING)
     logger = logging.getLogger(__name__)
 
     if not main_args.query:
         logger.error("Please provide one or more queries to run")
```

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/cli/simulator.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/cli/simulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import sys
 import argparse
 import logging
 from rich.logging import RichHandler
 import yaml
 
 from gaarf.io import writer, reader  # type: ignore
 from gaarf.simulation import simulate_data, SimulatorSpecification
-from .utils import GaarfConfigBuilder, ConfigSaver, initialize_runtime_parameters
+from .utils import GaarfConfigBuilder
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("query", nargs="+")
     parser.add_argument("-c", "--config", dest="gaarf_config", default=None)
     parser.add_argument("-s",
@@ -17,14 +18,15 @@
                         dest="simulator_config",
                         default=None)
     parser.add_argument("--account", dest="customer_id", default="None")
     parser.add_argument("--output", dest="save", default="console")
     parser.add_argument("--input", dest="input", default="file")
     parser.add_argument("--api-version", dest="api_version", default=12)
     parser.add_argument("--log", "--loglevel", dest="loglevel", default="info")
+    parser.add_argument("--logger", dest="logger", default="local")
     parser.add_argument("--customer-ids-query",
                         dest="customer_ids_query",
                         default=None)
     parser.add_argument("--customer-ids-query-file",
                         dest="customer_ids_query_file",
                         default=None)
     parser.add_argument("--save-config",
@@ -36,18 +38,25 @@
     parser.add_argument("--config-destination",
                         dest="save_config_dest",
                         default="config.yaml")
     parser.set_defaults(save_config=False)
     args = parser.parse_known_args()
     main_args = args[0]
 
-    logging.basicConfig(format="%(message)s",
-                        level=main_args.loglevel.upper(),
-                        datefmt="%Y-%m-%d %H:%M:%S",
-                        handlers=[RichHandler(rich_tracebacks=True)])
+    if main_args.logger == "rich":
+        logging.basicConfig(format="%(message)s",
+                            level=main_args.loglevel.upper(),
+                            datefmt="%Y-%m-%d %H:%M:%S",
+                            handlers=[RichHandler(rich_tracebacks=True)])
+    else:
+        logging.basicConfig(
+                    format="[%(asctime)s][%(name)s][%(levelname)s] %(message)s",
+                    stream=sys.stdout,
+                    level=main_args.loglevel.upper(),
+                    datefmt="%Y-%m-%d %H:%M:%S")
     logging.getLogger("google.ads.googleads.client").setLevel(logging.WARNING)
     logging.getLogger("smart_open.smart_open_lib").setLevel(logging.WARNING)
     logging.getLogger("urllib3.connectionpool").setLevel(logging.WARNING)
     logger = logging.getLogger(__name__)
 
     config = GaarfConfigBuilder(args).build()
     logger.debug("config: %s", config)
```

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/cli/utils.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/cli/utils.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/io/formatter.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/io/formatter.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/io/reader.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/io/reader.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/io/writer.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/io/writer.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/parsers.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections import abc
 from typing import Any, Dict, Tuple, Sequence, Union
 from operator import attrgetter
-import datetime
 import re
 import proto  # type: ignore
 from proto.marshal.collections.repeated import (  # type: ignore
     Repeated, RepeatedComposite)  # type: ignore
 from google.protobuf.internal.containers import (
     RepeatedScalarFieldContainer,
     RepeatedCompositeFieldContainer)  # type: ignore
@@ -86,21 +85,26 @@
             return "Not set"
         return super().parse(request)
 
 
 class GoogleAdsRowParser:
 
     def __init__(self, query_specification, nested_fields=None):
-        self.nested_fields = nested_fields
-        self.parser = self._init_parsers()
-        self.row_getter = attrgetter(*query_specification.fields)
         self.fields = query_specification.fields
+        self.nested_fields = nested_fields
         self.customizers = query_specification.customizers
         self.virtual_columns = query_specification.virtual_columns
         self.column_names = query_specification.column_names
+        self.parser = self._init_parsers()
+        self.row_getter = attrgetter(*query_specification.fields)
+        # Some segments are automatically converted to 0 when not present
+        # For this case we specify attribute `respect_null` which converts
+        # such attributes to None rather than 0
+        self.respect_nulls = ("segments.sk_ad_network_conversion_value"
+                              in self.fields)
 
     def _init_parsers(self):
         parser_chain = BaseParser(None)
         for parser in [
                 EmptyAttributeParser, AttributeParser, RepeatedCompositeParser,
                 RepeatedParser
         ]:
@@ -178,18 +182,32 @@
                     parsed_element = self.parser.parse(
                         extracted_attribute) or extracted_attribute
             final_rows.append(parsed_element)
         return final_rows if len(final_rows) > 1 else final_rows[0]
 
     def _get_attributes_from_row(self, row, getter) -> Tuple[Any, ...]:
         attributes = getter(row)
+        if self.respect_nulls:
+            # Validate whether field is actually present in a protobuf message
+            value = row.segments._pb.HasField("sk_ad_network_conversion_value")
+            # If not present
+            if not value:
+                # Convert to list to perform modification
+                attributes = list(attributes)
+                # Replace 0 attributes in the row with None
+                attributes[self.fields.index(
+                    "segments.sk_ad_network_conversion_value")] = None
+                # Convert back to tuple
+                attributes = tuple(attributes)
+        else:
+            attributes = getter(row)
         return attributes if isinstance(attributes, tuple) else (attributes, )
 
     def _convert_virtual_column(self, row,
-                                   virtual_column: VirtualColumn) -> str:
+                                virtual_column: VirtualColumn) -> str:
         if virtual_column.type == "built-in":
             return virtual_column.value
         elif virtual_column.type == "expression":
             virtual_column_getter = attrgetter(*virtual_column.fields)
             virtual_column_values = virtual_column_getter(row)
             try:
                 iter(virtual_column_values)
@@ -204,23 +222,21 @@
                 result = eval(
                     virtual_column.substitute_expression.format(
                         **virtual_column_replacements))
             except ZeroDivisionError:
                 return 0
             except TypeError:
                 raise VirtualColumnError(
-                    f"cannot parse virtual_column {virtual_column.value}"
-                )
+                    f"cannot parse virtual_column {virtual_column.value}")
             except Exception as e:
                 return virtual_column.value
             return result
         else:
             raise ValueError(
-                f"Unsupported virtual column type: {virtual_column_type}"
-            )
+                f"Unsupported virtual column type: {virtual_column_type}")
 
 
 class ResourceFormatter:
 
     @staticmethod
     def get_resource(element: str) -> str:
         return re.split(": ", str(element).strip())[1]
```

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/query_editor.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/query_editor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/query_executor.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/query_executor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/report.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/report.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,18 +66,19 @@
                 for row in self.results:
                     rows = []
                     for index in indices:
                         rows.append(row[index])
                     results.append(rows)
                 return cls(results, key)
             else:
-                non_existing_keys = set(key).intersection(set(self.column_names))
+                non_existing_keys = set(key).intersection(
+                    set(self.column_names))
                 if len(non_existing_keys) > 1:
-                    message =  f"Columns '{', '.join(list(non_existing_keys))}' cannot be found in the report"
-                message =  f"Column '{non_existing_keys.pop()}' cannot be found in the report"
+                    message = f"Columns '{', '.join(list(non_existing_keys))}' cannot be found in the report"
+                message = f"Column '{non_existing_keys.pop()}' cannot be found in the report"
                 raise TypeError(message)
         else:
             if key in self.column_names:
                 index = self.column_names.index(key)
                 results = [[row[index]] for row in self.results]
                 return cls(results, [key])
         if self.multi_column_report:
@@ -100,38 +101,49 @@
         if not isinstance(other, self.__class__):
             raise TypeError("Add operation is supported only for GaarfReport")
         if self.column_names != other.column_names:
             raise ValueError("column_names should be the same in GaarfReport")
         return GaarfReport(results=self.results + other.results,
                            column_names=self.column_names)
 
+    @classmethod
+    def from_pandas(cls, df: pd.DataFrame):
+        return cls(results=df.values.tolist(),
+                   column_names=list(df.columns.values))
+
 
 class GaarfRow:
 
     def __init__(self, data: Sequence[Union[int, float, str]],
                  column_names: Sequence[str]):
-        self.data = data
-        try:
-            self.n_elements = len(data)
-        except TypeError:
-            self.n_elements = 1
-        self.column_names = column_names
+        super().__setattr__("data", data)
+        super().__setattr__("column_names", column_names)
 
     def __getattr__(self, element: str) -> Any:
         if element in self.column_names:
             return self.data[self.column_names.index(element)]
         raise AttributeError(f"cannot find {element} element!")
 
     def __getitem__(self, element: Union[str, int]) -> Any:
-        if isinstance(element, int) and element < self.n_elements:
+        if isinstance(element, int) and element < len(self.column_names):
             return self.data[element]
         if isinstance(element, str):
             return self.__getattr__(element)
         raise IndexError(f"cannot find {element} element!")
 
+    def __setattr__(self, name: str, value: Union[str, int]) -> None:
+        self.__setitem__(name, value)
+
+    def __setitem__(self, name: str, value: Union[str, int]) -> None:
+        if name in self.column_names:
+            self.data[self.column_names.index(name)] = value
+        else:
+            self.data.append(value)
+            self.column_names.append(name)
+
     def get(self, item: str) -> Any:
         return self.__getattr__(item)
 
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
         if self.column_names != other.column_names:
```

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/simulation.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/simulation.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/gaarf/utils.py` & `google-ads-api-report-fetcher-1.5.0/gaarf/utils.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/PKG-INFO` & `google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ads-api-report-fetcher
-Version: 1.4.0
+Version: 1.5.0
 Summary: Library for fetching reports from Google Ads API and saving them locally / BigQuery.
 Home-page: https://github.com/google/ads-api-reports-fetcher
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt` & `google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/setup.py` & `google-ads-api-report-fetcher-1.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "sqlalchemy": ["sqlalchemy"],
     "simulator": ["Faker"]
 }
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     name="google-ads-api-report-fetcher",
-    version="1.4.0",
+    version="1.5.0",
     description=
     "Library for fetching reports from Google Ads API and saving them locally / BigQuery.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/google/ads-api-reports-fetcher",
     author="Google Inc. (gTech gPS CSE team)",
     author_email="no-reply@google.com",
@@ -38,11 +38,13 @@
     ],
     extras_require=EXTRAS_REQUIRE,
     setup_requires=["pytest-runner"],
     tests_requires=["pytest"],
     entry_points={
         "console_scripts": [
             "gaarf=gaarf.cli.gaarf:main",
+            "gaarf-py=gaarf.cli.gaarf:main",
             "gaarf-bq=gaarf.cli.bq:main",
+            "gaarf-py-bq=gaarf.cli.bq:main",
             "gaarf-simulator=gaarf.cli.simulator:main",
         ]
     })
```

### Comparing `google-ads-api-report-fetcher-1.4.0/tests/unit/test_base_query.py` & `google-ads-api-report-fetcher-1.5.0/tests/unit/test_base_query.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/tests/unit/test_bq_executor.py` & `google-ads-api-report-fetcher-1.5.0/tests/unit/test_bq_executor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/tests/unit/test_cli_utils.py` & `google-ads-api-report-fetcher-1.5.0/tests/unit/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/tests/unit/test_parsers.py` & `google-ads-api-report-fetcher-1.5.0/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/tests/unit/test_query_editor.py` & `google-ads-api-report-fetcher-1.5.0/tests/unit/test_query_editor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/tests/unit/test_reader.py` & `google-ads-api-report-fetcher-1.5.0/tests/unit/test_reader.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/tests/unit/test_report.py` & `google-ads-api-report-fetcher-1.5.0/tests/unit/test_report.py`

 * *Files 22% similar despite different names*

```diff
@@ -168,7 +168,38 @@
     assert new_report == [1, 2]
 
 
 def test_slicing_multi_column_gaarf_report_returns_element(
         single_column_report):
     new_report = single_column_report[0]
     assert new_report == [1]
+
+
+def test_set_non_existing_item_gaarf_row_get_new_column(multi_column_report):
+    row = multi_column_report[0]
+    row["campaign_id_new"] = row["campaign_id"] * 100
+    assert row == GaarfRow(
+        data=[1, 2, 100],
+        column_names=["campaign_id", "ad_group_id", "campaign_id_new"])
+
+
+def test_set_existing_item_gaarf_row_updates_column(multi_column_report):
+    row = multi_column_report[0]
+    row["campaign_id"] = row["campaign_id"] * 100
+    assert row == GaarfRow(data=[100, 2],
+                           column_names=["campaign_id", "ad_group_id"])
+
+
+def test_set_non_existing_attribute_gaarf_row_get_new_column(
+        multi_column_report):
+    row = multi_column_report[0]
+    row.campaign_id_new = row.campaign_id * 100
+    assert row == GaarfRow(
+        data=[1, 2, 100],
+        column_names=["campaign_id", "ad_group_id", "campaign_id_new"])
+
+
+def test_set_existing_attribute_gaarf_row_updates_column(multi_column_report):
+    row = multi_column_report[0]
+    row.campaign_id = row.campaign_id * 100
+    assert row == GaarfRow(data=[100, 2],
+                           column_names=["campaign_id", "ad_group_id"])
```

### Comparing `google-ads-api-report-fetcher-1.4.0/tests/unit/test_simulation.py` & `google-ads-api-report-fetcher-1.5.0/tests/unit/test_simulation.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.4.0/tests/unit/test_writer.py` & `google-ads-api-report-fetcher-1.5.0/tests/unit/test_writer.py`

 * *Files identical despite different names*


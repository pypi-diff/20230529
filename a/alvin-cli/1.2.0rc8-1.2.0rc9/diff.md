# Comparing `tmp/alvin_cli-1.2.0rc8.tar.gz` & `tmp/alvin_cli-1.2.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alvin_cli-1.2.0rc8.tar", last modified: Thu Oct 13 11:42:29 2022, max compression
+gzip compressed data, was "alvin_cli-1.2.0rc9.tar", last modified: Fri Oct 21 10:59:57 2022, max compression
```

## Comparing `alvin_cli-1.2.0rc8.tar` & `alvin_cli-1.2.0rc9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 11:42:29.878463 alvin_cli-1.2.0rc8/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-10-13 11:42:29.878463 alvin_cli-1.2.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 11:42:29.878463 alvin_cli-1.2.0rc8/alvin_cli/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 11:42:29.878463 alvin_cli-1.2.0rc8/alvin_cli/config/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/config/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/config/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4349 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/config_management.py
--rw-r--r--   0 runner    (1001) docker     (121)    18872 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     3631 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/impact_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     8672 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/manual_lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 11:42:29.878463 alvin_cli-1.2.0rc8/alvin_cli/platforms/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28038 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/platforms/add.py
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/platforms/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 11:42:29.878463 alvin_cli-1.2.0rc8/alvin_cli/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/schemas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 11:42:29.878463 alvin_cli-1.2.0rc8/alvin_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/utils/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    14683 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/utils/check_sql_impact_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    10235 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/utils/common_arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/utils/dbt_compile.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/utils/dbt_deps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6052 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/utils/git_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    11659 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/utils/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12958 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/alvin_cli/utils/utils_dbt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 11:42:29.878463 alvin_cli-1.2.0rc8/alvin_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-10-13 11:42:29.000000 alvin_cli-1.2.0rc8/alvin_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-10-13 11:42:29.000000 alvin_cli-1.2.0rc8/alvin_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 11:42:29.000000 alvin_cli-1.2.0rc8/alvin_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-13 11:42:29.000000 alvin_cli-1.2.0rc8/alvin_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-13 11:42:29.000000 alvin_cli-1.2.0rc8/alvin_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-13 11:42:29.000000 alvin_cli-1.2.0rc8/alvin_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-10-13 11:42:29.882463 alvin_cli-1.2.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-13 11:41:48.000000 alvin_cli-1.2.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:59:57.213184 alvin_cli-1.2.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-10-21 10:59:57.213184 alvin_cli-1.2.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:59:57.209184 alvin_cli-1.2.0rc9/alvin_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:59:57.213184 alvin_cli-1.2.0rc9/alvin_cli/config/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/config/loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/config/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4349 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/config_management.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18872 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/impact_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8672 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/manual_lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:59:57.213184 alvin_cli-1.2.0rc9/alvin_cli/platforms/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28038 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/platforms/add.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/platforms/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:59:57.213184 alvin_cli-1.2.0rc9/alvin_cli/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/schemas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:59:57.213184 alvin_cli-1.2.0rc9/alvin_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/utils/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16091 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/utils/check_sql_impact_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10235 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/utils/common_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3549 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/utils/dbt_compile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/utils/dbt_deps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6052 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/utils/git_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12142 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/utils/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12958 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/alvin_cli/utils/utils_dbt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:59:57.213184 alvin_cli-1.2.0rc9/alvin_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-10-21 10:59:57.000000 alvin_cli-1.2.0rc9/alvin_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-10-21 10:59:57.000000 alvin_cli-1.2.0rc9/alvin_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 10:59:57.000000 alvin_cli-1.2.0rc9/alvin_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-21 10:59:57.000000 alvin_cli-1.2.0rc9/alvin_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-21 10:59:57.000000 alvin_cli-1.2.0rc9/alvin_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-21 10:59:57.000000 alvin_cli-1.2.0rc9/alvin_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-10-21 10:59:57.213184 alvin_cli-1.2.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 10:59:17.000000 alvin_cli-1.2.0rc9/setup.py
```

### Comparing `alvin_cli-1.2.0rc8/LICENSE` & `alvin_cli-1.2.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/PKG-INFO` & `alvin_cli-1.2.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alvin_cli
-Version: 1.2.0rc8
+Version: 1.2.0rc9
 Summary: Alvin CLI
 Home-page: https://github.com/alvindotai/alvin
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `alvin_cli-1.2.0rc8/README.md` & `alvin_cli-1.2.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/cli.py` & `alvin_cli-1.2.0rc9/alvin_cli/cli.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/config/loader.py` & `alvin_cli-1.2.0rc9/alvin_cli/config/loader.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/config/settings.py` & `alvin_cli-1.2.0rc9/alvin_cli/config/settings.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/config_management.py` & `alvin_cli-1.2.0rc9/alvin_cli/config_management.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/entity.py` & `alvin_cli-1.2.0rc9/alvin_cli/entity.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/impact_analysis.py` & `alvin_cli-1.2.0rc9/alvin_cli/impact_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import logging
 from typing import List
 
 import typer
+from alvin_api_client.model.impact_analysis_node_list_response import (
+    ImpactAnalysisNodeListResponse,
+)
 from alvin_api_client.model.impact_analysis_platform_request import (
     ImpactAnalysisPlatformRequest,
 )
 from alvin_api_client.model.impact_analysis_query_request import (
     ImpactAnalysisQueryRequest,
 )
 from alvin_api_client.model.impact_analysis_request import ImpactAnalysisRequest
@@ -75,17 +78,17 @@
             platform=ImpactAnalysisPlatformRequest(id=platform_id),
         )
 
         query_validation_response = default_api.validate_impact_analysis_query_api_v2_impact_analysis_validate_query_post(
             request_in_query_validate
         )
 
-        if query_validation_response["is_valid_query"]:
+        if query_validation_response.is_valid_query:
 
-            impact_analysis_response = default_api.run_impact_node_query_api_v2_impact_analysis_query_string_nodes_post(
+            impact_analysis_response: ImpactAnalysisNodeListResponse = default_api.run_impact_node_query_api_v2_impact_analysis_query_string_nodes_post(
                 request_in_query_validate
             )
 
             print_node_stats_impact_analysis(impact_analysis_response)
 
             if save_to_file:
                 structured_data = structure_impact_analysis_data(
```

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/manual_lineage.py` & `alvin_cli-1.2.0rc9/alvin_cli/manual_lineage.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/platforms/add.py` & `alvin_cli-1.2.0rc9/alvin_cli/platforms/add.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/platforms/platform.py` & `alvin_cli-1.2.0rc9/alvin_cli/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/schemas/models.py` & `alvin_cli-1.2.0rc9/alvin_cli/schemas/models.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/utils/api_client.py` & `alvin_cli-1.2.0rc9/alvin_cli/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/utils/check_sql_impact_analysis.py` & `alvin_cli-1.2.0rc9/alvin_cli/utils/check_sql_impact_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,35 +5,39 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 
 import pandas as pd
+from alvin_api_client.model.impact_analysis_node_list_response import (
+    ImpactAnalysisNodeListResponse,
+)
 from alvin_api_client.model.impact_analysis_platform_request import (
     ImpactAnalysisPlatformRequest,
 )
 from alvin_api_client.model.impact_analysis_query_request import (
     ImpactAnalysisQueryRequest,
 )
 from alvin_api_client.model.impact_analysis_request import ImpactAnalysisRequest
-from alvin_api_client.model.impact_analysis_response import ImpactAnalysisResponse
 from rich.console import Console
 from sqlfluff.core import FluffConfig
 from sqlfluff_templater_dbt.templater import DbtTemplater
 from tabulate import tabulate
 
 from alvin_cli.config import settings
 from alvin_cli.schemas.models import FileGitHistory
 from alvin_cli.schemas.models import GitChangeType
 from alvin_cli.schemas.models import ImpactAnalysisCLIReport
 from alvin_cli.schemas.models import Model
 from alvin_cli.utils.api_client import default_api
 from alvin_cli.utils.dbt_compile import main as dbt_compile
 from alvin_cli.utils.dbt_deps import main as dbt_deps
+from alvin_cli.utils.helper_functions import extract_dict
+from alvin_cli.utils.helper_functions import handle_print_exception
 from alvin_cli.utils.helper_functions import print_node_stats_impact_analysis
 from alvin_cli.utils.utils_dbt import ERROR_RETURN_CODE
 from alvin_cli.utils.utils_dbt import get_json
 from alvin_cli.utils.utils_dbt import get_model_sqls
 from alvin_cli.utils.utils_dbt import get_models
 from alvin_cli.utils.utils_dbt import num_of_days_from_now
 
@@ -76,17 +80,22 @@
 
     console.print(header_text, style="bold yellow")
 
     all_status_code = 0
     for model in models:
         # We run all, but we need to store if
         # any model execution failed
-        status_code = __process_model(model, status_code, report)
-        if status_code:
-            all_status_code = status_code
+        try:
+            status_code = __process_model(model, status_code, report)
+            if status_code:
+                all_status_code = status_code
+        except Exception as e:
+            exception = e.__str__()
+            handle_print_exception(extract_dict(exception), exception[:5])
+            all_status_code = 1
 
     report.status_code = all_status_code
 
     with open("report.json", "w") as f:
         json.dump(report.dict(), f, ensure_ascii=False)
 
     return all_status_code
@@ -254,15 +263,15 @@
     return dbt_create_as_str
 
 
 def __call_impact_analysis_api(
     dbt_create_as_str: str,
     node: Dict[str, Any],
     file_git_history: Optional[FileGitHistory],
-) -> ImpactAnalysisResponse:
+) -> ImpactAnalysisNodeListResponse:
     impact_analysis_query_request = ImpactAnalysisQueryRequest(
         source_text=dbt_create_as_str
     )
     impact_analysis_platform_request = ImpactAnalysisPlatformRequest(
         id=settings.alvin_platform_id
     )
     impact_analysis_request = ImpactAnalysisRequest(
@@ -279,15 +288,15 @@
             previous_model_name = file_git_history.previous_model_name
             if model_name != previous_model_name:
                 renamed_entity_id = (
                     f"{node['database']}.{node['schema']}.{previous_model_name}"
                 )
                 impact_analysis_query_request.renamed_entity_id = renamed_entity_id
 
-    response: ImpactAnalysisResponse = default_api.run_impact_node_query_api_v2_impact_analysis_query_string_nodes_post(
+    response: ImpactAnalysisNodeListResponse = default_api.run_impact_node_query_api_v2_impact_analysis_query_string_nodes_post(
         impact_analysis_request
     )
 
     if settings.alvin_verbose_log:
         print(
             f"DEBUG: The impact analysis request sent is \n\n {impact_analysis_request}"
         )
@@ -318,52 +327,72 @@
             original_file_path, relation_name, node["config"]
         )
 
         response = __call_impact_analysis_api(dbt_create_as_str, node, None)
 
         console.print(f"Changed Entity: [underline]{relation_name}", style="bold")
 
-        impact_analysis_response = response.impact_analysis_response
-        query_report = impact_analysis_response.query_report
-
-        report.markdown_text = report.markdown_text + f"\n## {relation_name}"
-        if query_report:
-
-            query_report_url_code = query_report.query_report_url_code
-            report_url = __create_report_url(query_report_url_code)
-            wide_console.print(f"└──FULL REPORT: {report_url}", overflow="ellipsis")
-            report.markdown_text = (
-                report.markdown_text
-                + f"\n[![RUN](https://alvin-public-assets.s3.eu-central-1.amazonaws.com/run.svg)]"
-                f"({report_url})\n"
+        if response:
+            impact_analysis_response: ImpactAnalysisNodeListResponse = (
+                response.impact_analysis_response
             )
-        else:
-            report.markdown_text = report.markdown_text + "\n\n"
+            query_report = impact_analysis_response.query_report
 
-        console.print("\n\n")
+            report.markdown_text = report.markdown_text + f"\n## {relation_name}"
+            if query_report:
 
-        report_stats = print_node_stats_impact_analysis(response)
+                query_report_url_code = query_report.query_report_url_code
+                report_url = __create_report_url(query_report_url_code)
+                wide_console.print(f"└──FULL REPORT: {report_url}", overflow="ellipsis")
+                report.markdown_text = (
+                    report.markdown_text
+                    + f"\n[![RUN](https://alvin-public-assets.s3.eu-central-1.amazonaws.com/run.svg)]"
+                    f"({report_url})\n"
+                )
+            else:
+                report.markdown_text = report.markdown_text + "\n\n"
 
-        report.markdown_text = (
-            report.markdown_text
-            + f"\n <b>{report_stats.total_impacted_assets}</b> assets and <b>{report_stats.total_impacted_users}</b> people impacted \n\n\n"
-        )
-        rows = []
+            console.print("\n\n")
 
-        for platform, impact in report_stats.impact_per_platform.items():
-            impact_stats = ""
-            for impact_status, count in impact.items():
-                impact_stats += f"{count}:{impact_status.title()}  "
-            rows.append({"Platform ID": platform, "Impact Status ": impact_stats})
-        df = pd.DataFrame(rows)
-
-        report.markdown_text = (
-            report.markdown_text
-            + f"\n {tabulate(df, headers= 'keys', tablefmt='github', showindex=False)}"
-        )
+            report_stats = print_node_stats_impact_analysis(response)
+            if report_stats:
+                report.markdown_text = (
+                    report.markdown_text
+                    + f"\n <b>{report_stats.total_impacted_assets}</b> assets and <b>{report_stats.total_impacted_users}</b> people impacted \n\n\n"
+                )
+                rows = []
+
+                for platform, impact in report_stats.impact_per_platform.items():
+                    impact_stats = ""
+                    for impact_status, count in impact.items():
+                        impact_stats += f"{count}:{impact_status.title()}  "
+                    rows.append(
+                        {"Platform ID": platform, "Impact Status ": impact_stats}
+                    )
+                df = pd.DataFrame(rows)
+
+                report.markdown_text = (
+                    report.markdown_text
+                    + f"\n {tabulate(df, headers= 'keys', tablefmt='github', showindex=False)}"
+                )
+            else:
+                if response and impact_analysis_response:
+                    if settings.alvin_verbose_log:
+                        error_message = impact_analysis_response.get("errorMessage")
+                        if error_message:
+                            print(
+                                f"Error returned from Impact Analysis: {error_message}. "
+                            )
+                status_code = 1
+                print(
+                    f"Unable to process `{model.model_id}` impact analysis response. "
+                )
+        else:
+            status_code = 1
+            print(f"Unable to process `{model.model_id}` impact analysis response. ")
 
     else:
         status_code = 1
         print(f"Invalid model `{model.model_id}` in manifest file. ")
     return status_code
```

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/utils/common_arguments.py` & `alvin_cli-1.2.0rc9/alvin_cli/utils/common_arguments.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/utils/dbt_compile.py` & `alvin_cli-1.2.0rc9/alvin_cli/utils/dbt_compile.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,16 +77,16 @@
                     *cmd_flags,
                     "--profiles-dir",
                     dbt_profiles_dir,
                 ]
 
     except Exception as e:
         if settings.alvin_verbose_log:
-            print(f"DEBUG! dbt target : {dbt_target}")
-            print(f"DEBUG! dbt profile dir : {dbt_profiles_dir}")
+            print(f"DEBUG dbt target : {dbt_target}")
+            print(f"DEBUG dbt profile dir : {dbt_profiles_dir}")
             print(f"Exception raised is: {e}")
 
     return cmd
 
 
 def main(argv: Optional[Sequence[str]] = None) -> int:
     parser = argparse.ArgumentParser()
```

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/utils/git_metadata.py` & `alvin_cli-1.2.0rc9/alvin_cli/utils/git_metadata.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/utils/helper_functions.py` & `alvin_cli-1.2.0rc9/alvin_cli/utils/helper_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from typing import Sequence
 from typing import Tuple
 
 import pandas as pd
 import ruamel.yaml
 import typer
 import yaml
+from alvin_api_client.model.impact_analysis_node_list_response import (
+    ImpactAnalysisNodeListResponse,
+)
 from rich.console import Console
 from rich.table import Table
 
 from alvin_cli.config import settings
 from alvin_cli.schemas.models import ReportStats
 from alvin_cli.utils.common_arguments import BRIGHT_BLUE_COLOR_TYPER
 from alvin_cli.utils.common_arguments import BRIGHT_CYAN_COLOR_TYPER
@@ -225,53 +228,65 @@
 
         usage_stats_in_list.append(usage_stats_in_dict)
 
     return usage_stats_in_list, user_name_stats
 
 
 def print_node_stats_impact_analysis(
-    impact_analysis_data: dict,
-) -> ReportStats:
+    impact_analysis_data: ImpactAnalysisNodeListResponse,
+) -> Optional[ReportStats]:
 
-    node_stats = impact_analysis_data["node_stats"]
-    impact_per_platform = node_stats["impact_per_platform"]
-    impacted_users = node_stats["impacted_users"]
-    total_impacted_assets = sum(node_stats["entity_types"].values())
-    total_impacted_users = len(impacted_users)
+    node_stats = impact_analysis_data.node_stats
+    if not node_stats:
+        return None
+
+    impact_per_platform = node_stats.impact_per_platform
+    impacted_users = node_stats.impacted_users
+
+    total_impacted_users = 0
+    if impacted_users:
+        total_impacted_users = len(impacted_users)
+
+    total_impacted_assets = 0
+    if node_stats.entity_types:
+        total_impacted_assets = sum(node_stats.entity_types.values())
 
     typer.secho(
         "\n------------ Summary of Impacted Entities ------------\n",
         fg=BRIGHT_GREEN_COLOR_TYPER,
     )
 
     typer.secho(
         f"{total_impacted_assets} assets and {total_impacted_users} people impacted",
         fg=BRIGHT_YELLOW_COLOR_TYPER,
     )
 
-    typer.secho(
-        f'   Impacted Number of Columns : {node_stats["entity_types"].get("COLUMN", 0)}',
-        fg=BRIGHT_CYAN_COLOR_TYPER,
-    )
-    typer.secho(
-        f'   Impacted Number of Tables : {node_stats["entity_types"].get("TABLE", 0)}',
-        fg=BRIGHT_YELLOW_COLOR_TYPER,
-    )
-    typer.secho(
-        f'   Impact Status Direct :  {node_stats["impact_status"].get("DIRECT", 0)}',
-        fg=BRIGHT_MAGENTA_COLOR_TYPER,
-    )
-    typer.secho(
-        f'   Impact Status Breaking Change : {node_stats["impact_status"].get("BREAKING", 0)}',
-        fg=BRIGHT_MAGENTA_COLOR_TYPER,
-    )
-    typer.secho(
-        f'   Impact Status Stale : {node_stats["impact_status"].get("STALE", 0)}',
-        fg=BRIGHT_MAGENTA_COLOR_TYPER,
-    )
+    if node_stats.entity_types:
+        typer.secho(
+            f'   Impacted Number of Columns : {node_stats.entity_types.get("COLUMN", 0)}',
+            fg=BRIGHT_CYAN_COLOR_TYPER,
+        )
+        typer.secho(
+            f'   Impacted Number of Tables : {node_stats.entity_types.get("TABLE", 0)}',
+            fg=BRIGHT_YELLOW_COLOR_TYPER,
+        )
+
+    if node_stats.impact_status:
+        typer.secho(
+            f'   Impact Status Direct :  {node_stats.impact_status.get("DIRECT", 0)}',
+            fg=BRIGHT_MAGENTA_COLOR_TYPER,
+        )
+        typer.secho(
+            f'   Impact Status Breaking Change : {node_stats.impact_status.get("BREAKING", 0)}',
+            fg=BRIGHT_MAGENTA_COLOR_TYPER,
+        )
+        typer.secho(
+            f'   Impact Status Stale : {node_stats.impact_status.get("STALE", 0)}',
+            fg=BRIGHT_MAGENTA_COLOR_TYPER,
+        )
 
     if impacted_users:
         typer.secho(
             "   Impacted Users :",
             fg=BRIGHT_CYAN_COLOR_TYPER,
         )
         for user, count in impacted_users.items():
@@ -281,41 +296,42 @@
             )
 
     typer.secho(
         "\n------------ Impact Per Platform Id ------------\n",
         fg=BRIGHT_GREEN_COLOR_TYPER,
     )
 
-    for platform, impact in impact_per_platform.items():
-        typer.secho(f"{platform}", fg=BRIGHT_YELLOW_COLOR_TYPER)
-        for impact_status, count in impact.items():
-            typer.secho(f"   {impact_status} : {count}", fg=BRIGHT_BLUE_COLOR_TYPER)
+    if impact_per_platform:
+        for platform, impact in impact_per_platform.items():
+            typer.secho(f"{platform}", fg=BRIGHT_YELLOW_COLOR_TYPER)
+            for impact_status, count in impact.items():
+                typer.secho(f"   {impact_status} : {count}", fg=BRIGHT_BLUE_COLOR_TYPER)
 
     return ReportStats(
         impact_per_platform=impact_per_platform,
         impacted_users=impacted_users,
         total_impacted_assets=total_impacted_assets,
         total_impacted_users=total_impacted_users,
     )
 
 
 def structure_impact_analysis_data(
-    impact_analysis_data: dict,
+    impact_analysis_data: ImpactAnalysisNodeListResponse,
 ) -> list:
     """Format the Impact Analysis Data, returns list of dicts"""
 
     structured_data_list = []
-    impact_analysis_response = impact_analysis_data["impact_analysis_response"]
-    query_entities = impact_analysis_response["query_entities"]
+    impact_analysis_response = impact_analysis_data.impact_analysis_response
+    query_entities = impact_analysis_response.query_entities
 
     if query_entities:
         for impacted_entity in query_entities:
             structured_data_dict = {
-                "entityType": str(impacted_entity.get("entityType")),
-                "entityId": impacted_entity.get("entityId"),
+                "entityType": str(impacted_entity.entityType),
+                "entityId": impacted_entity.entityId,
             }
             structured_data_list.append(structured_data_dict)
 
     return structured_data_list
 
 
 def read_config_from_json(config: Path) -> Optional[dict]:
```

### Comparing `alvin_cli-1.2.0rc8/alvin_cli/utils/utils_dbt.py` & `alvin_cli-1.2.0rc9/alvin_cli/utils/utils_dbt.py`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/alvin_cli.egg-info/PKG-INFO` & `alvin_cli-1.2.0rc9/alvin_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alvin-cli
-Version: 1.2.0rc8
+Version: 1.2.0rc9
 Summary: Alvin CLI
 Home-page: https://github.com/alvindotai/alvin
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `alvin_cli-1.2.0rc8/alvin_cli.egg-info/SOURCES.txt` & `alvin_cli-1.2.0rc9/alvin_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alvin_cli-1.2.0rc8/setup.cfg` & `alvin_cli-1.2.0rc9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alvin_cli
-version = 1.2.0rc8
+version = 1.2.0rc9
 description = Alvin CLI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alvindotai/alvin
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.7
```


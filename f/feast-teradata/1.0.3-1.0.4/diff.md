# Comparing `tmp/feast-teradata-1.0.3.tar.gz` & `tmp/feast-teradata-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feast-teradata-1.0.3.tar", last modified: Fri Jan 27 12:03:47 2023, max compression
+gzip compressed data, was "feast-teradata-1.0.4.tar", last modified: Mon May 29 21:22:49 2023, max compression
```

## Comparing `feast-teradata-1.0.3.tar` & `feast-teradata-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:47.189859 feast-teradata-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-01-27 12:03:47.189859 feast-teradata-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:47.189859 feast-teradata-1.0.3/feast_teradata/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-27 12:03:45.000000 feast-teradata-1.0.3/feast_teradata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:47.189859 feast-teradata-1.0.3/feast_teradata/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:47.185859 feast-teradata-1.0.3/feast_teradata/cli/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:47.189859 feast-teradata-1.0.3/feast_teradata/cli/template/teradata/
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/cli/template/teradata/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:47.189859 feast-teradata-1.0.3/feast_teradata/cli/template/teradata/feature_repo/
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/cli/template/teradata/feature_repo/driver_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/cli/template/teradata/feature_repo/feature_store.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/cli/template/teradata/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:47.189859 feast-teradata-1.0.3/feast_teradata/offline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/offline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24110 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/offline/teradata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/offline/teradata_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:47.189859 feast-teradata-1.0.3/feast_teradata/online/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/online/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/online/teradata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/feast_teradata/teradata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 12:03:47.189859 feast-teradata-1.0.3/feast_teradata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-01-27 12:03:47.000000 feast-teradata-1.0.3/feast_teradata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-27 12:03:47.000000 feast-teradata-1.0.3/feast_teradata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 12:03:47.000000 feast-teradata-1.0.3/feast_teradata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-27 12:03:47.000000 feast-teradata-1.0.3/feast_teradata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-27 12:03:47.000000 feast-teradata-1.0.3/feast_teradata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-27 12:03:47.000000 feast-teradata-1.0.3/feast_teradata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-27 12:03:47.189859 feast-teradata-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-27 12:03:01.000000 feast-teradata-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:22:49.966155 feast-teradata-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-29 21:22:49.966155 feast-teradata-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:22:49.962155 feast-teradata-1.0.4/feast_teradata/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 21:22:48.000000 feast-teradata-1.0.4/feast_teradata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:22:49.962155 feast-teradata-1.0.4/feast_teradata/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:22:49.962155 feast-teradata-1.0.4/feast_teradata/cli/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:22:49.962155 feast-teradata-1.0.4/feast_teradata/cli/template/teradata/
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/cli/template/teradata/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:22:49.962155 feast-teradata-1.0.4/feast_teradata/cli/template/teradata/feature_repo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/cli/template/teradata/feature_repo/driver_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/cli/template/teradata/feature_repo/feature_store.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/cli/template/teradata/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:22:49.962155 feast-teradata-1.0.4/feast_teradata/offline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/offline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/offline/teradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/offline/teradata_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:22:49.966155 feast-teradata-1.0.4/feast_teradata/online/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/online/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/online/teradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/feast_teradata/teradata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:22:49.962155 feast-teradata-1.0.4/feast_teradata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-29 21:22:49.000000 feast-teradata-1.0.4/feast_teradata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-29 21:22:49.000000 feast-teradata-1.0.4/feast_teradata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 21:22:49.000000 feast-teradata-1.0.4/feast_teradata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-29 21:22:49.000000 feast-teradata-1.0.4/feast_teradata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 21:22:49.000000 feast-teradata-1.0.4/feast_teradata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 21:22:49.000000 feast-teradata-1.0.4/feast_teradata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-29 21:22:49.966155 feast-teradata-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-29 21:21:59.000000 feast-teradata-1.0.4/setup.py
```

### Comparing `feast-teradata-1.0.3/LICENSE` & `feast-teradata-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feast-teradata-1.0.3/LICENSE-3RD-PARTY.txt` & `feast-teradata-1.0.4/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `feast-teradata-1.0.3/PKG-INFO` & `feast-teradata-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feast-teradata
-Version: 1.0.3
+Version: 1.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/Teradata/feast-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8,<3.11
@@ -130,22 +130,32 @@
 ```
 
 To configure Teradata as the `Registry`, configure the `registry_type` as `sql` and the path as the sqlalchemy url for teradata as follows
 ```yaml
 registry:
     registry_type: sql
     path: teradatasql://<user>:<password>@<host>/?database=<database>&LOGMECH=<TDNEGO|LDAP|etc>
+    cache_ttl_seconds: 120
 ```
 
 ## Release Notes
 
+### 1.0.4
+
+- Update: bump Feast dependency to 0.31.1 
+
+### 1.0.3
+
+- Fix: Added string mapping for columns. 
+
 ### 1.0.2
 
 - Doc: Improve README with details on repo configuration
 - Fix: Fix Github Release on CI Release
+- Fix: Updated path variable to become OS independent.
 
 ### 1.0.1
 
 - Doc: Improve README with better getting started information. 
 - Fix: Remove pytest from requirements.txt
 - Fix: Set minimum python version to 3.8 due to feast dependency on pandas>=1.4.3
 - Fix: Updated feast-td types conversion
```

### Comparing `feast-teradata-1.0.3/README.md` & `feast-teradata-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,22 +116,32 @@
 ```
 
 To configure Teradata as the `Registry`, configure the `registry_type` as `sql` and the path as the sqlalchemy url for teradata as follows
 ```yaml
 registry:
     registry_type: sql
     path: teradatasql://<user>:<password>@<host>/?database=<database>&LOGMECH=<TDNEGO|LDAP|etc>
+    cache_ttl_seconds: 120
 ```
 
 ## Release Notes
 
+### 1.0.4
+
+- Update: bump Feast dependency to 0.31.1 
+
+### 1.0.3
+
+- Fix: Added string mapping for columns. 
+
 ### 1.0.2
 
 - Doc: Improve README with details on repo configuration
 - Fix: Fix Github Release on CI Release
+- Fix: Updated path variable to become OS independent.
 
 ### 1.0.1
 
 - Doc: Improve README with better getting started information. 
 - Fix: Remove pytest from requirements.txt
 - Fix: Set minimum python version to 3.8 due to feast dependency on pandas>=1.4.3
 - Fix: Updated feast-td types conversion
```

### Comparing `feast-teradata-1.0.3/feast_teradata/cli/cli.py` & `feast-teradata-1.0.4/feast_teradata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `feast-teradata-1.0.3/feast_teradata/cli/template/teradata/bootstrap.py` & `feast-teradata-1.0.4/feast_teradata/cli/template/teradata/bootstrap.py`

 * *Files identical despite different names*

### Comparing `feast-teradata-1.0.3/feast_teradata/cli/template/teradata/feature_repo/driver_repo.py` & `feast-teradata-1.0.4/feast_teradata/cli/template/teradata/feature_repo/driver_repo.py`

 * *Files identical despite different names*

### Comparing `feast-teradata-1.0.3/feast_teradata/cli/template/teradata/feature_repo/feature_store.yaml` & `feast-teradata-1.0.4/feast_teradata/cli/template/teradata/feature_repo/feature_store.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 project: my_project
 registry:
     registry_type: sql
     path: Teradata registry path
+    cache_ttl_seconds: 120
 provider: local
 online_store:
     type: feast_teradata.online.teradata.TeradataOnlineStore
     host: Teradata host URL
     database: Teradata database
     user: Teradata user
     password: Teradata password
@@ -13,8 +14,8 @@
 offline_store:
     type: feast_teradata.offline.teradata.TeradataOfflineStore
     host: Teradata host URL
     database: Teradata database
     user: Teradata user
     password: Teradata password
     log_mech: Teradata log_mech
-entity_key_serialization_version: 2
+entity_key_serialization_version: 2
```

### Comparing `feast-teradata-1.0.3/feast_teradata/cli/template/teradata/test_workflow.py` & `feast-teradata-1.0.4/feast_teradata/cli/template/teradata/test_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         "\n--- Historical features for batch scoring (all entities in a window using SQL entity dataframe) ---"
     )
     fetch_historical_features_entity_sql(store, for_batch_scoring=True)
 
     print("\n--- Load features into online store ---")
     store.materialize_incremental(end_date=datetime.now())
 
+    print("\n--- Refreshing registry ---")
+    store.refresh_registry()
+
     print("\n--- Online features ---")
     fetch_online_features(store)
 
     print("\n--- Online features retrieved (instead) through a feature service---")
     fetch_online_features(store, source="feature_service")
 
     print(
```

### Comparing `feast-teradata-1.0.3/feast_teradata/offline/teradata.py` & `feast-teradata-1.0.4/feast_teradata/offline/teradata.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,23 +284,23 @@
     def full_feature_names(self) -> bool:
         return self._full_feature_names
 
     @property
     def on_demand_feature_views(self) -> List[OnDemandFeatureView]:
         return self._on_demand_feature_views
 
-    def _to_df_internal(self) -> pd.DataFrame:
+    def _to_df_internal(self, timeout: Optional[int] = None) -> pd.DataFrame:
         # We use arrow format because it gives better control of the table schema
         return self._to_arrow_internal().to_pandas()
 
     def to_sql(self) -> str:
         with self._query_generator() as query:
             return query
 
-    def _to_arrow_internal(self) -> pa.Table:
+    def _to_arrow_internal(self, timeout: Optional[int] = None) -> pa.Table:
         with self._query_generator() as query:
             with get_conn(self.config.offline_store).raw_connection().cursor() as cur:
                 cur.execute(query)
                 fields = [
                     (c[0], teradata_type_to_feast_value_type(c[1]))
                     for c in cur.description
                 ]
```

### Comparing `feast-teradata-1.0.3/feast_teradata/offline/teradata_source.py` & `feast-teradata-1.0.4/feast_teradata/offline/teradata_source.py`

 * *Files identical despite different names*

### Comparing `feast-teradata-1.0.3/feast_teradata/online/teradata.py` & `feast-teradata-1.0.4/feast_teradata/online/teradata.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
             if not res:
                 result.append((None, None))
             else:
                 result.append((res_ts, res))
         return result
 
-    @log_exceptions_and_usage(online_store="snowflake")
+    @log_exceptions_and_usage(online_store="teradata")
     def update(
             self,
             config: RepoConfig,
             tables_to_delete: Sequence[FeatureView],
             tables_to_keep: Sequence[FeatureView],
             entities_to_delete: Sequence[Entity],
             entities_to_keep: Sequence[Entity],
```

### Comparing `feast-teradata-1.0.3/feast_teradata/teradata_utils.py` & `feast-teradata-1.0.4/feast_teradata/teradata_utils.py`

 * *Files identical despite different names*

### Comparing `feast-teradata-1.0.3/feast_teradata.egg-info/PKG-INFO` & `feast-teradata-1.0.4/feast_teradata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feast-teradata
-Version: 1.0.3
+Version: 1.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/Teradata/feast-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8,<3.11
@@ -130,22 +130,32 @@
 ```
 
 To configure Teradata as the `Registry`, configure the `registry_type` as `sql` and the path as the sqlalchemy url for teradata as follows
 ```yaml
 registry:
     registry_type: sql
     path: teradatasql://<user>:<password>@<host>/?database=<database>&LOGMECH=<TDNEGO|LDAP|etc>
+    cache_ttl_seconds: 120
 ```
 
 ## Release Notes
 
+### 1.0.4
+
+- Update: bump Feast dependency to 0.31.1 
+
+### 1.0.3
+
+- Fix: Added string mapping for columns. 
+
 ### 1.0.2
 
 - Doc: Improve README with details on repo configuration
 - Fix: Fix Github Release on CI Release
+- Fix: Updated path variable to become OS independent.
 
 ### 1.0.1
 
 - Doc: Improve README with better getting started information. 
 - Fix: Remove pytest from requirements.txt
 - Fix: Set minimum python version to 3.8 due to feast dependency on pandas>=1.4.3
 - Fix: Updated feast-td types conversion
```

### Comparing `feast-teradata-1.0.3/feast_teradata.egg-info/SOURCES.txt` & `feast-teradata-1.0.4/feast_teradata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feast-teradata-1.0.3/setup.py` & `feast-teradata-1.0.4/setup.py`

 * *Files identical despite different names*


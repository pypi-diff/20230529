# Comparing `tmp/caveclient-5.6.0.tar.gz` & `tmp/caveclient-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caveclient-5.6.0.tar", last modified: Thu May 18 12:51:20 2023, max compression
+gzip compressed data, was "caveclient-5.7.0.tar", last modified: Mon May 29 21:18:30 2023, max compression
```

## Comparing `caveclient-5.6.0.tar` & `caveclient-5.7.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-18 12:51:20.446744 caveclient-5.6.0/
--rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.6.0/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-18 12:51:20.446462 caveclient-5.6.0/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.6.0/README.rst
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-18 12:51:20.432311 caveclient-5.6.0/caveclient/
--rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-05-18 12:51:16.000000 caveclient-5.6.0/caveclient/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.6.0/caveclient/annotationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.6.0/caveclient/auth.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.6.0/caveclient/base.py
--rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.6.0/caveclient/chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.6.0/caveclient/datastack_lookup.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.6.0/caveclient/emannotationschemas.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.6.0/caveclient/endpoints.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2407 2023-05-10 16:28:45.000000 caveclient-5.6.0/caveclient/format_utils.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.6.0/caveclient/frameworkclient.py
--rw-r--r--   0 forrestc   (503) staff       (20)    16314 2023-05-10 16:28:45.000000 caveclient-5.6.0/caveclient/infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.6.0/caveclient/jsonservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.6.0/caveclient/l2cache.py
--rw-r--r--   0 forrestc   (503) staff       (20)    91156 2023-05-18 12:51:11.000000 caveclient-5.6.0/caveclient/materializationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.6.0/caveclient/session_config.py
--rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.6.0/caveclient/timeit.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-18 12:51:20.436399 caveclient-5.6.0/caveclient/tools/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.6.0/caveclient/tools/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.6.0/caveclient/tools/caching.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.6.0/caveclient/tools/stage.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-18 12:51:20.435900 caveclient-5.6.0/caveclient.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-18 12:51:20.000000 caveclient-5.6.0/caveclient.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-05-18 12:51:20.000000 caveclient-5.6.0/caveclient.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-05-18 12:51:20.000000 caveclient-5.6.0/caveclient.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      119 2023-05-18 12:51:20.000000 caveclient-5.6.0/caveclient.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-05-18 12:51:20.000000 caveclient-5.6.0/caveclient.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      118 2023-05-10 03:33:26.000000 caveclient-5.6.0/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-05-18 12:51:20.446811 caveclient-5.6.0/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.6.0/setup.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-18 12:51:20.442340 caveclient-5.6.0/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.6.0/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.6.0/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.6.0/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.6.0/tests/test_chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.6.0/tests/test_infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.6.0/tests/test_materialization.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-29 21:18:30.933795 caveclient-5.7.0/
+-rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.7.0/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-29 21:18:30.929004 caveclient-5.7.0/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.7.0/README.rst
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-29 21:18:30.900091 caveclient-5.7.0/caveclient/
+-rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-05-29 21:17:44.000000 caveclient-5.7.0/caveclient/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.7.0/caveclient/annotationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.7.0/caveclient/auth.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.7.0/caveclient/base.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    39464 2023-05-29 21:15:16.000000 caveclient-5.7.0/caveclient/chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.7.0/caveclient/datastack_lookup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.7.0/caveclient/emannotationschemas.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.7.0/caveclient/endpoints.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2407 2023-05-10 16:28:45.000000 caveclient-5.7.0/caveclient/format_utils.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.7.0/caveclient/frameworkclient.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    16314 2023-05-10 16:28:45.000000 caveclient-5.7.0/caveclient/infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.7.0/caveclient/jsonservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.7.0/caveclient/l2cache.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    91183 2023-05-19 22:16:03.000000 caveclient-5.7.0/caveclient/materializationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      778 2023-05-19 14:30:34.000000 caveclient-5.7.0/caveclient/mytimer.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.7.0/caveclient/session_config.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-29 21:18:30.911890 caveclient-5.7.0/caveclient/tools/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.7.0/caveclient/tools/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.7.0/caveclient/tools/caching.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.7.0/caveclient/tools/stage.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-29 21:18:30.905964 caveclient-5.7.0/caveclient.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-29 21:18:30.000000 caveclient-5.7.0/caveclient.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      870 2023-05-29 21:18:30.000000 caveclient-5.7.0/caveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-05-29 21:18:30.000000 caveclient-5.7.0/caveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      119 2023-05-29 21:18:30.000000 caveclient-5.7.0/caveclient.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-05-29 21:18:30.000000 caveclient-5.7.0/caveclient.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      118 2023-05-10 03:33:26.000000 caveclient-5.7.0/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-05-29 21:18:30.934331 caveclient-5.7.0/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.7.0/setup.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-29 21:18:30.918129 caveclient-5.7.0/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.7.0/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.7.0/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.7.0/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.7.0/tests/test_chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.7.0/tests/test_infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.7.0/tests/test_materialization.py
```

### Comparing `caveclient-5.6.0/README.rst` & `caveclient-5.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/annotationengine.py` & `caveclient-5.7.0/caveclient/annotationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/auth.py` & `caveclient-5.7.0/caveclient/auth.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/base.py` & `caveclient-5.7.0/caveclient/base.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/chunkedgraph.py` & `caveclient-5.7.0/caveclient/chunkedgraph.py`

 * *Files 5% similar despite different names*

```diff
@@ -836,14 +836,83 @@
         r = handle_response(
             self.session.post(
                 url, data=json.dumps(data, cls=BaseEncoder), params=query_d
             )
         )
         return np.array(r["is_latest"], bool)
 
+    def suggest_latest_roots(
+        self,
+        root_id,
+        timestamp=None,
+        stop_layer=None,
+        return_all=False,
+        return_fraction_overlap=False,
+    ):
+        """Suggest latest roots for a given root id, based on overlap of component chunk ids.
+        Note that edits change chunk ids, and so this effectively measures the fraction of unchanged chunks
+        at a given chunk layer, which sets the size scale of chunks. Higher layers are coarser.
+
+        Parameters
+        ----------
+        root_id : int64
+            Root id of the potentially outdated object.
+        timestamp : datetime, optional
+            Datetime at which "latest" roots are being computed, by default None. If None, the current time is used.
+            Note that this has to be a timestamp after the creation of the root_id.
+        stop_layer : int, optional
+            Chunk level at which to compute overlap, by default None.
+            No value will take the 4th from the top layer, which emphasizes speed and works well for larger objects.
+            Lower values are slower but more fine-grained.
+            Values under 2 (i.e. supervoxels) are not recommended except in extremely fine grained scenarios.
+        return_all : bool, optional
+            If True, return all current ids sorted from most overlap to least, by default False. If False, only the top is returned.
+        return_fraction_overlap : bool, optional
+            If True, return all fractions sorted by most overlap to least, by default False. If False, only the topmost value is returned.
+        """
+        curr_ids = self.get_latest_roots(root_id, timestamp_future=timestamp)
+        if root_id in curr_ids:
+            if return_all:
+                if return_fraction_overlap:
+                    return [root_id], [1]
+                else:
+                    return [root_id]
+            else:
+                if return_fraction_overlap:
+                    return root_id, 1
+                else:
+                    return root_id
+
+        delta_layers = 4
+        if stop_layer is None:
+            stop_layer = self.segmentation_info.get("graph", {}).get("n_layers", 6) - delta_layers
+        stop_layer = max(1, stop_layer)
+        
+        chunks_orig = self.get_leaves(root_id, stop_layer=stop_layer)
+        chunk_list = np.array(
+            [
+                len(
+                    np.intersect1d(
+                        chunks_orig,
+                        self.get_leaves(oid, stop_layer=stop_layer),
+                        assume_unique=True,
+                    )
+                )
+                / len(chunks_orig)
+                for oid in curr_ids
+            ]
+        )
+        order = np.argsort(chunk_list)[::-1]
+        if not return_all:
+            order = order[0]
+        if return_fraction_overlap:
+            return curr_ids[order], chunk_list[order]
+        else:
+            return curr_ids[order]
+
     def is_valid_nodes(self, node_ids, start_timestamp=None, end_timestamp=None):
         """Check whether nodes are valid for given timestamp range
 
         Valid is defined as existing in the chunkedgraph. This makes no statement
         about these IDs being roots, supervoxel or anything in-between. It also
         does not take into account whether a root id has since been edited.
```

### Comparing `caveclient-5.6.0/caveclient/datastack_lookup.py` & `caveclient-5.7.0/caveclient/datastack_lookup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/emannotationschemas.py` & `caveclient-5.7.0/caveclient/emannotationschemas.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/endpoints.py` & `caveclient-5.7.0/caveclient/endpoints.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/format_utils.py` & `caveclient-5.7.0/caveclient/format_utils.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/frameworkclient.py` & `caveclient-5.7.0/caveclient/frameworkclient.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/infoservice.py` & `caveclient-5.7.0/caveclient/infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/jsonservice.py` & `caveclient-5.7.0/caveclient/jsonservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/l2cache.py` & `caveclient-5.7.0/caveclient/l2cache.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/materializationengine.py` & `caveclient-5.7.0/caveclient/materializationengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from urllib.error import HTTPError
 import warnings
 import pytz
 import pandas as pd
 from IPython.display import HTML
-from .timeit import TimeIt
+from .mytimer import MyTimeIt
 from typing import Union, Iterable
 import itertools
 import pyarrow as pa
 from datetime import datetime, timezone
 import numpy as np
 import json
 from .endpoints import materialization_api_versions, materialization_common
@@ -937,15 +937,15 @@
             future_map = None
 
         if future_map is not None:
             # pyarrow can make dataframes read only. Copying resets that.
             df = df.copy()
 
         sv_columns = [c for c in df.columns if c.endswith("supervoxel_id")]
-        with TimeIt("is_latest_roots"):
+        with MyTimeIt("is_latest_roots"):
             all_root_ids = np.empty(0, dtype=np.int64)
 
             # go through the columns and collect all the root_ids to check
             # to see if they need updating
             for sv_col in sv_columns:
                 root_id_col = sv_col[: -len("supervoxel_id")] + "root_id"
                 # use the future map to update rootIDs
@@ -966,39 +966,39 @@
             latest_root_ids = np.concatenate([[0], latest_root_ids])
 
             # go through the columns and collect all the supervoxel ids to update
             all_svids = np.empty(0, dtype=np.int64)
             all_is_latest = []
             all_svid_lengths = []
             for sv_col in sv_columns:
-                with TimeIt(f"find svids {sv_col}"):
+                with MyTimeIt(f"find svids {sv_col}"):
                     root_id_col = sv_col[: -len("supervoxel_id")] + "root_id"
                     svids = df[sv_col].values
                     root_ids = df[root_id_col]
                     is_latest_root = np.isin(root_ids, latest_root_ids)
                     all_is_latest.append(is_latest_root)
                     n_svids = len(svids[~is_latest_root])
                     all_svid_lengths.append(n_svids)
                     logger.info(f"{sv_col} has {n_svids} to update")
                     all_svids = np.append(all_svids, svids[~is_latest_root])
         logger.info(f"num zero svids: {np.sum(all_svids==0)}")
         logger.info(f"all_svids dtype {all_svids.dtype}")
         logger.info(f"all_svid_lengths {all_svid_lengths}")
-        with TimeIt("get_roots"):
+        with MyTimeIt("get_roots"):
             # find the up to date root_ids for those supervoxels
             updated_root_ids = self.cg_client.get_roots(all_svids, timestamp=timestamp)
             del all_svids
 
         # loop through the columns again replacing the root ids with their updated
         # supervoxelids
         k = 0
         for is_latest_root, n_svids, sv_col in zip(
             all_is_latest, all_svid_lengths, sv_columns
         ):
-            with TimeIt(f"replace_roots {sv_col}"):
+            with MyTimeIt(f"replace_roots {sv_col}"):
                 root_id_col = sv_col[: -len("supervoxel_id")] + "root_id"
                 root_ids = df[root_id_col].values.copy()
 
                 uroot_id = updated_root_ids[k : k + n_svids]
                 k += n_svids
                 root_ids[~is_latest_root] = uroot_id
                 # ran into an isssue with pyarrow producing read only columns
@@ -1199,15 +1199,15 @@
             verify=self.verify,
         )
         self.raise_for_status(response)
 
         if desired_resolution is None:
             desired_resolution = self.desired_resolution
 
-        with TimeIt("deserialize"):
+        with MyTimeIt("deserialize"):
             with warnings.catch_warnings():
                 warnings.simplefilter(action="ignore", category=FutureWarning)
                 warnings.simplefilter(action="ignore", category=DeprecationWarning)
                 df = pa.deserialize(response.content)
                 df = df.copy()
                 if desired_resolution is not None:
 
@@ -1323,15 +1323,15 @@
         if self.cg_client is None:
             raise ValueError("You must have a cg_client to run live_query")
 
         if datastack_name is None:
             datastack_name = self.datastack_name
         if desired_resolution is None:
             desired_resolution = self.desired_resolution
-        with TimeIt("find_mat_version"):
+        with MyTimeIt("find_mat_version"):
             # we want to find the most recent materialization
             # in which the timestamp given is in the future
             mds = self.get_versions_metadata()
             materialization_version = None
             # make sure the materialization's are increasing in ID/time
             for md in sorted(mds, key=lambda x: x["id"]):
                 ts = md["time_stamp"]
@@ -1366,15 +1366,15 @@
                         """The timestamp you passed is not recent enough
                 for the materialization versions that are available"""
                     )
                 )
 
         # first we want to translate all these filters into the IDss at the
         # most recent materialization
-        with TimeIt("map_filters"):
+        with MyTimeIt("map_filters"):
             past_filters, future_map = self.map_filters(
                 [filter_in_dict, filter_out_dict, filter_equal_dict],
                 timestamp,
                 timestamp_start,
             )
             past_filter_in_dict, past_filter_out_dict, past_equal_dict = past_filters
             if past_equal_dict is not None:
@@ -1390,15 +1390,15 @@
                         past_filter_in_dict[col] = past_equal_dict.pop(col)
                 if len(past_equal_dict) == 0:
                     past_equal_dict = None
 
         tables, suffix_map = self._resolve_merge_reference(
             merge_reference, table, datastack_name, materialization_version
         )
-        with TimeIt("package query"):
+        with MyTimeIt("package query"):
             url, data, query_args, encoding = self._format_query_components(
                 datastack_name,
                 materialization_version,
                 tables,
                 select_columns,
                 suffix_map,
                 {table: past_filter_in_dict}
@@ -1415,15 +1415,15 @@
                 True,
                 offset,
                 limit,
                 desired_resolution,
             )
             logger.debug(f"query_args: {query_args}")
             logger.debug(f"query data: {data}")
-        with TimeIt("query materialize"):
+        with MyTimeIt("query materialize"):
             response = self.session.post(
                 url,
                 data=json.dumps(data, cls=BaseEncoder),
                 headers={
                     "Content-Type": "application/json",
                     "Accept-Encoding": encoding,
                 },
@@ -1432,15 +1432,15 @@
                 verify=self.verify,
             )
             self.raise_for_status(response)
 
         if desired_resolution is None:
             desired_resolution = self.desired_resolution
 
-        with TimeIt("deserialize"):
+        with MyTimeIt("deserialize"):
             with warnings.catch_warnings():
                 warnings.simplefilter(action="ignore", category=FutureWarning)
                 warnings.simplefilter(action="ignore", category=DeprecationWarning)
                 df = pa.deserialize(response.content)
                 df = df.copy()
                 if desired_resolution is not None:
                     if not response.headers.get("dataframe_resolution", None):
@@ -1461,15 +1461,15 @@
         # post process the dataframe to update all the root_ids columns
         # with the most up to date get roots
         df = self._update_rootids(df, timestamp, future_map)
 
         # apply the original filters to remove rows
         # from this result which are not relevant
         if post_filter:
-            with TimeIt("post_filter"):
+            with MyTimeIt("post_filter"):
                 if filter_in_dict is not None:
                     for col, val in filter_in_dict.items():
                         df = df[df[col].isin(val)]
                 if filter_out_dict is not None:
                     for col, val in filter_out_dict.items():
                         df = df[~df[col].isin(val)]
                 if filter_equal_dict is not None:
@@ -1853,15 +1853,15 @@
             },
             params=query_args,
             stream=~return_df,
             verify=self.verify,
         )
         self.raise_for_status(response)
 
-        with TimeIt("deserialize"):
+        with MyTimeIt("deserialize"):
             with warnings.catch_warnings():
                 warnings.simplefilter(action="ignore", category=FutureWarning)
                 warnings.simplefilter(action="ignore", category=DeprecationWarning)
                 df = pa.deserialize(response.content)
                 df = df.copy()
                 if desired_resolution is not None:
                     if not response.headers.get("dataframe_resolution", None):
```

### Comparing `caveclient-5.6.0/caveclient/session_config.py` & `caveclient-5.7.0/caveclient/session_config.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/timeit.py` & `caveclient-5.7.0/caveclient/mytimer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from time import time
-import builtins
 import logging
+
 logger = logging.getLogger(__name__)
 
+
 indent = 0
 
 
-class TimeIt:
+class MyTimeIt:
     def __init__(self, message="", *args, **kwargs):
         self._message = message
         self._args = args
         self._kwargs = kwargs
         self._start = None
 
     def __enter__(self):
```

### Comparing `caveclient-5.6.0/caveclient/tools/caching.py` & `caveclient-5.7.0/caveclient/tools/caching.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient/tools/stage.py` & `caveclient-5.7.0/caveclient/tools/stage.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/caveclient.egg-info/SOURCES.txt` & `caveclient-5.7.0/caveclient.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 caveclient/endpoints.py
 caveclient/format_utils.py
 caveclient/frameworkclient.py
 caveclient/infoservice.py
 caveclient/jsonservice.py
 caveclient/l2cache.py
 caveclient/materializationengine.py
+caveclient/mytimer.py
 caveclient/session_config.py
-caveclient/timeit.py
 caveclient.egg-info/PKG-INFO
 caveclient.egg-info/SOURCES.txt
 caveclient.egg-info/dependency_links.txt
 caveclient.egg-info/requires.txt
 caveclient.egg-info/top_level.txt
 caveclient/tools/__init__.py
 caveclient/tools/caching.py
```

### Comparing `caveclient-5.6.0/setup.py` & `caveclient-5.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/tests/conftest.py` & `caveclient-5.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/tests/test_annotation.py` & `caveclient-5.7.0/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/tests/test_chunkedgraph.py` & `caveclient-5.7.0/tests/test_chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/tests/test_infoservice.py` & `caveclient-5.7.0/tests/test_infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.6.0/tests/test_materialization.py` & `caveclient-5.7.0/tests/test_materialization.py`

 * *Files identical despite different names*


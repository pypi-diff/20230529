# Comparing `tmp/autobricks-0.5.0.tar.gz` & `tmp/autobricks-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobricks-0.5.0.tar", last modified: Fri May  5 20:01:49 2023, max compression
+gzip compressed data, was "autobricks-0.6.0.tar", last modified: Mon May 29 09:10:37 2023, max compression
```

## Comparing `autobricks-0.5.0.tar` & `autobricks-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 20:01:49.493501 autobricks-0.5.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-05-05 20:01:49.493501 autobricks-0.5.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     7157 2023-05-05 20:01:28.000000 autobricks-0.5.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 20:01:49.493501 autobricks-0.5.0/autobricks/
--rw-r--r--   0 vsts      (1001) docker     (123)     8987 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/Cluster.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3545 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/Dbfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4815 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/Job.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1395 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/Library.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7619 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/SetupTools.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12859 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/Sql.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8297 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/Workspace.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/_common.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1266 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/_decode_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 20:01:49.493501 autobricks-0.5.0/autobricks/api_service/
--rw-r--r--   0 vsts      (1001) docker     (123)      439 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/api_service/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5017 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/api_service/_auth.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1440 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/api_service/_auth_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1686 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/api_service/_base_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2876 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/api_service/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/api_service/_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4363 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/api_service/api_service.py
--rw-r--r--   0 vsts      (1001) docker     (123)      312 2023-05-05 20:01:28.000000 autobricks-0.5.0/autobricks/api_service/autobricks_logging.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 20:01:49.493501 autobricks-0.5.0/autobricks.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-05-05 20:01:49.000000 autobricks-0.5.0/autobricks.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      723 2023-05-05 20:01:49.000000 autobricks-0.5.0/autobricks.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-05 20:01:49.000000 autobricks-0.5.0/autobricks.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-05 20:01:49.000000 autobricks-0.5.0/autobricks.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-05 20:01:49.000000 autobricks-0.5.0/autobricks.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-05-05 20:01:49.000000 autobricks-0.5.0/autobricks.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-05 20:01:49.493501 autobricks-0.5.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1076 2023-05-05 20:01:28.000000 autobricks-0.5.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-29 09:10:37.208781 autobricks-0.6.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-05-29 09:10:37.208781 autobricks-0.6.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     7157 2023-05-29 09:10:10.000000 autobricks-0.6.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-29 09:10:37.204781 autobricks-0.6.0/autobricks/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8987 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/Cluster.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3545 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/Dbfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5762 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/Job.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1395 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/Library.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7619 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/SetupTools.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12859 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/Sql.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8297 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/Workspace.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/_common.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1266 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/_decode_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-29 09:10:37.208781 autobricks-0.6.0/autobricks/api_service/
+-rw-r--r--   0 vsts      (1001) docker     (123)      439 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/api_service/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5017 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/api_service/_auth.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1440 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/api_service/_auth_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1686 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/api_service/_base_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2876 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/api_service/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/api_service/_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4363 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/api_service/api_service.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      312 2023-05-29 09:10:10.000000 autobricks-0.6.0/autobricks/api_service/autobricks_logging.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-29 09:10:37.204781 autobricks-0.6.0/autobricks.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-05-29 09:10:37.000000 autobricks-0.6.0/autobricks.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      723 2023-05-29 09:10:37.000000 autobricks-0.6.0/autobricks.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-29 09:10:37.000000 autobricks-0.6.0/autobricks.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-29 09:10:37.000000 autobricks-0.6.0/autobricks.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-29 09:10:37.000000 autobricks-0.6.0/autobricks.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-05-29 09:10:37.000000 autobricks-0.6.0/autobricks.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-29 09:10:37.208781 autobricks-0.6.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1076 2023-05-29 09:10:10.000000 autobricks-0.6.0/setup.py
```

### Comparing `autobricks-0.5.0/PKG-INFO` & `autobricks-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobricks
-Version: 0.5.0
+Version: 0.6.0
 Summary: Databricks Deployment Utils
 Home-page: https://autobricks.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/autobricks
 Project-URL: Documentation, https://autobricks.readthedocs.io/en/latest/
```

### Comparing `autobricks-0.5.0/README.md` & `autobricks-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/Cluster.py` & `autobricks-0.6.0/autobricks/Cluster.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/Dbfs.py` & `autobricks-0.6.0/autobricks/Dbfs.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/Job.py` & `autobricks-0.6.0/autobricks/Job.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,14 +97,26 @@
         )
     except Exception:
         raise JobException(name)
 
     return response
 
 
+def job_reset(job: dict):
+    name = job.get("name", "Unknown")
+    try:
+        response = _api_service.api_post(
+            endpoint, "reset", job, api_version=_JOBS_API_VERSION
+        )
+    except Exception:
+        raise JobException(name)
+
+    return response
+
+
 def job_delete(job_id: int):
     data = {"job_id": job_id}
     try:
         response = _api_service.api_post(
             endpoint, "delete", data, api_version=_JOBS_API_VERSION
         )
     except Exception:
@@ -156,35 +168,61 @@
         job_id = jobs[0].get("job_id", False)
         return job_id
     else:
         return None
 
 
 def job_recreate(job: dict):
-    name = job.get("name", "Unknown")
+    try:
+        name = job["name"]
+    except KeyError as e:
+        raise Exception(f"Job definition doesn't have a {e}.")
 
     job_id = job_get_id(name)
     _logger.info(f"Recreating job {name} job_id={job_id}")
 
     if job_id:
         _logger.info(f"deleting job {name} job_id={job_id}")
         job_delete(job_id=job_id)
 
     _logger.info(f"creating new job {name}")
     job_create(job=job)
 
 
-def job_import_jobs(from_path: str, tags: Union[str, List[str], None] = None):
+def job_create_or_replace(job: dict):
+    try:
+        name = job["name"]
+    except KeyError as e:
+        raise Exception(f"Job definition doesn't have a {e}.")
+
+    job_id = job_get_id(name)
+
+    if job_id:
+        _logger.info(f"updaing job {name} job_id={job_id}")
+        job["new_settings"] = job
+        job["job_id"] = job_id
+        job_delete(job_id=job_id)
+    else:
+        _logger.info(f"creating new job {name}")
+        job_create(job=job)
+
+
+def job_import_jobs(
+    from_path: str, tags: Union[str, List[str], None] = None, recreate: bool = False
+):
     for root, _, files in os.walk(from_path):
         config_files = [f for f in files if get_metadata_format(f)]
 
         for f in config_files:
             filename = os.path.join(root, f)
             filename = os.path.abspath(filename)
             with open(filename, "r", encoding="utf-8") as f:
                 metadata_format = get_metadata_format(filename)
                 data: dict = load_format(f, metadata_format)
 
             in_tags = data.get("tags")
 
             if tags_exist_in(tags, in_tags):
-                job_recreate(data)
+                if recreate:
+                    job_recreate(data)
+                else:
+                    job_create_or_replace(data)
```

### Comparing `autobricks-0.5.0/autobricks/Library.py` & `autobricks-0.6.0/autobricks/Library.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/SetupTools.py` & `autobricks-0.6.0/autobricks/SetupTools.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/Sql.py` & `autobricks-0.6.0/autobricks/Sql.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/Workspace.py` & `autobricks-0.6.0/autobricks/Workspace.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/_common.py` & `autobricks-0.6.0/autobricks/_common.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/_decode_utils.py` & `autobricks-0.6.0/autobricks/_decode_utils.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/api_service/_auth.py` & `autobricks-0.6.0/autobricks/api_service/_auth.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/api_service/_auth_factory.py` & `autobricks-0.6.0/autobricks/api_service/_auth_factory.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/api_service/_base_api.py` & `autobricks-0.6.0/autobricks/api_service/_base_api.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/api_service/_configuration.py` & `autobricks-0.6.0/autobricks/api_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/api_service/_exceptions.py` & `autobricks-0.6.0/autobricks/api_service/_exceptions.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks/api_service/api_service.py` & `autobricks-0.6.0/autobricks/api_service/api_service.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/autobricks.egg-info/PKG-INFO` & `autobricks-0.6.0/autobricks.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobricks
-Version: 0.5.0
+Version: 0.6.0
 Summary: Databricks Deployment Utils
 Home-page: https://autobricks.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/autobricks
 Project-URL: Documentation, https://autobricks.readthedocs.io/en/latest/
```

### Comparing `autobricks-0.5.0/autobricks.egg-info/SOURCES.txt` & `autobricks-0.6.0/autobricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autobricks-0.5.0/setup.py` & `autobricks-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "PYPI.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="autobricks",
-    version="0.5.0",
+    version="0.6.0",
     description="Databricks Deployment Utils",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://autobricks.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/autobricks',
         'Documentation': 'https://autobricks.readthedocs.io/en/latest/'
```


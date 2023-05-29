# Comparing `tmp/airflow_mcd-0.1.0.tar.gz` & `tmp/airflow_mcd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow_mcd-0.1.0.tar", last modified: Fri May 26 20:09:12 2023, max compression
+gzip compressed data, was "dist/airflow_mcd-0.1.1.tar", last modified: Mon May 29 14:17:18 2023, max compression
```

## Comparing `airflow_mcd-0.1.0.tar` & `airflow_mcd-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/.circleci/README
--rw-r--r--   0 root         (0) root         (0)     3102 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1818 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1129 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     7468 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/README-dev.md
--rw-r--r--   0 root         (0) root         (0)     6655 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/airflow_mcd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/airflow_mcd/callbacks/
--rw-r--r--   0 root         (0) root         (0)     5575 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/callbacks/client.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/callbacks/mcd_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     4695 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/airflow_mcd/hooks/
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2773 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/hooks/session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/airflow_mcd/operators/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/operators/base_operator.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/airflow_mcd/operators/circuit_breaker_operators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/airflow_mcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7468 2023-05-26 20:09:12.000000 airflow_mcd-0.1.0/airflow_mcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      980 2023-05-26 20:09:12.000000 airflow_mcd-0.1.0/airflow_mcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 20:09:12.000000 airflow_mcd-0.1.0/airflow_mcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-26 20:09:12.000000 airflow_mcd-0.1.0/airflow_mcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-26 20:09:12.000000 airflow_mcd-0.1.0/airflow_mcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/examples/
--rw-r--r--   0 root         (0) root         (0)     2050 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/examples/sample_circuit_dag.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-26 20:09:12.883684 airflow_mcd-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1483 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/tests/callbacks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10706 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/callbacks/test_callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/hooks/test_session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:09:12.879684 airflow_mcd-0.1.0/tests/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/operators/test_base_op.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-05-26 20:08:14.000000 airflow_mcd-0.1.0/tests/operators/test_circuit_breaker_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.350695 airflow_mcd-0.1.1/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/.circleci/README
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.350695 airflow_mcd-0.1.1/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/README-dev.md
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.350695 airflow_mcd-0.1.1/airflow_mcd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/airflow_mcd/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     6669 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/callbacks/client.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/callbacks/mcd_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     4695 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/airflow_mcd/hooks/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/hooks/session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/airflow_mcd/operators/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/operators/base_operator.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/airflow_mcd/operators/circuit_breaker_operators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.350695 airflow_mcd-0.1.1/airflow_mcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-05-29 14:17:18.000000 airflow_mcd-0.1.1/airflow_mcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-29 14:17:18.000000 airflow_mcd-0.1.1/airflow_mcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 14:17:18.000000 airflow_mcd-0.1.1/airflow_mcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-29 14:17:18.000000 airflow_mcd-0.1.1/airflow_mcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 14:17:18.000000 airflow_mcd-0.1.1/airflow_mcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/examples/
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/examples/sample_circuit_dag.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/tests/callbacks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12943 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/hooks/test_session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:17:18.354695 airflow_mcd-0.1.1/tests/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/operators/test_base_op.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-05-29 14:16:02.000000 airflow_mcd-0.1.1/tests/operators/test_circuit_breaker_op.py
```

### Comparing `airflow_mcd-0.1.0/.circleci/config.yml` & `airflow_mcd-0.1.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/.gitignore` & `airflow_mcd-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/LICENSE` & `airflow_mcd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/Makefile` & `airflow_mcd-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/PKG-INFO` & `airflow_mcd-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_mcd
-Version: 0.1.0
+Version: 0.1.1
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.1.0/README-dev.md` & `airflow_mcd-0.1.1/README-dev.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/README.md` & `airflow_mcd-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/airflow_mcd/callbacks/client.py` & `airflow_mcd-0.1.1/airflow_mcd/callbacks/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,24 +10,63 @@
 from sgqlc.types import Variable, non_null
 
 from airflow_mcd.hooks import SessionHook
 
 
 logger = logging.getLogger(__name__)
 
+_ENV_MAPPINGS = {
+    'env_name': [
+        'AIRFLOW_ENV_NAME',                     # AWS
+        'COMPOSER_ENVIRONMENT',                 # GCP Composer
+        'AIRFLOW__WEBSERVER__INSTANCE_NAME',    # Astronomer
+    ],
+    'env_id': [
+        'AIRFLOW_ENV_ID',                       # AWS
+        'COMPOSER_GKE_NAME',                    # GCP Composer
+        'ASTRO_DEPLOYMENT_ID',                  # Astronomer
+    ],
+    'version': [
+        'AIRFLOW_VERSION',                      # AWS
+        'MAJOR_VERSION',                        # GCP Composer
+        'ASTRONOMER_RUNTIME_VERSION',           # Astronomer
+    ],
+    'base_url': [
+        'AIRFLOW__WEBSERVER__BASE_URL',         # available in all containers
+    ]
+}
+
+
+def _get_env_value(key: str, default_value: Optional[str] = None) -> Optional[str]:
+    for env_var in _ENV_MAPPINGS[key]:
+        value = os.environ.get(env_var)
+        if value:
+            return value
+    return default_value
+
 
 @dataclass_json
 @dataclass
 class AirflowEnv:
     # these env vars are used to get additional information about the Airflow
-    # environment when running in AWS or GCP.
-    env_name: str = os.environ.get('AIRFLOW_ENV_NAME', os.environ.get('COMPOSER_ENVIRONMENT', 'airflow'))
-    env_id: Optional[str] = os.environ.get('AIRFLOW_ENV_ID', os.environ.get('COMPOSER_GKE_NAME'))
-    version: Optional[str] = os.environ.get('AIRFLOW_VERSION', os.environ.get('MAJOR_VERSION'))
-    base_url: Optional[str] = os.environ.get('AIRFLOW__WEBSERVER__BASE_URL')
+    # environment when running in AWS, GCP or Astronomer.
+    env_name: str = ""
+    env_id: Optional[str] = None
+    version: Optional[str] = None
+    base_url: Optional[str] = None
+
+    def __post_init__(self):
+        if not self.env_name:
+            self.env_name = _get_env_value('env_name', 'airflow')
+        if not self.env_id:
+            self.env_id = _get_env_value('env_id')
+        if not self.version:
+            self.version = _get_env_value('version')
+        if not self.base_url:
+            self.base_url = _get_env_value('base_url')
 
 
 @dataclass_json
 @dataclass
 class DagTaskInstanceResult:
     task_id: str
     state: str
```

### Comparing `airflow_mcd-0.1.0/airflow_mcd/callbacks/mcd_callbacks.py` & `airflow_mcd-0.1.1/airflow_mcd/callbacks/mcd_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/airflow_mcd/callbacks/utils.py` & `airflow_mcd-0.1.1/airflow_mcd/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/airflow_mcd/hooks/session_hook.py` & `airflow_mcd-0.1.1/airflow_mcd/hooks/session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/airflow_mcd/operators/base_operator.py` & `airflow_mcd-0.1.1/airflow_mcd/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/airflow_mcd/operators/circuit_breaker_operators.py` & `airflow_mcd-0.1.1/airflow_mcd/operators/circuit_breaker_operators.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/airflow_mcd.egg-info/PKG-INFO` & `airflow_mcd-0.1.1/airflow_mcd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-mcd
-Version: 0.1.0
+Version: 0.1.1
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.1.0/airflow_mcd.egg-info/SOURCES.txt` & `airflow_mcd-0.1.1/airflow_mcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/examples/sample_circuit_dag.py` & `airflow_mcd-0.1.1/examples/sample_circuit_dag.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/setup.py` & `airflow_mcd-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/tests/callbacks/test_callbacks.py` & `airflow_mcd-0.1.1/tests/callbacks/test_callbacks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import os
 from datetime import datetime, timedelta
 from typing import Dict, List, Optional
 from unittest import TestCase
 from unittest.mock import create_autospec, patch
 
 import pytz
 from airflow import DAG
 from airflow.models import DagRun, TaskInstance, SlaMiss
 from sgqlc.types import Variable
 
-from airflow_mcd.callbacks.client import AirflowEventsClient
+from airflow_mcd.callbacks.client import AirflowEventsClient, AirflowEnv
 from airflow_mcd.callbacks.utils import AirflowEventsClientUtils
 
 
 # needed to have a successful assert_called_with as Variable doesn't implement __eq__
 class EqVariable(Variable):
     def __eq__(self, other):
         return other.name == self.name
@@ -83,14 +84,71 @@
                         "timestamp": m.timestamp.isoformat(),
                     }
                     for m in sla_misses
                 ]
             }
         )
 
+    def test_env_loading(self):
+        no_env = AirflowEnv()
+        self.assertEqual("airflow", no_env.env_name)
+        self.assertIsNone(no_env.env_id)
+        self.assertIsNone(no_env.version)
+        self.assertIsNone(no_env.base_url)
+
+        # AWS
+        with patch.dict(os.environ, {
+            "AIRFLOW_ENV_NAME": "aws_env_name",
+            "AIRFLOW_ENV_ID": "aws_env_id",
+            "AIRFLOW_VERSION": "aws_version",
+            "AIRFLOW__WEBSERVER__BASE_URL": "aws_url",
+        }):
+            env = AirflowEnv()
+            self.assertEqual("aws_env_name", env.env_name)
+            self.assertEqual("aws_env_id", env.env_id)
+            self.assertEqual("aws_version", env.version)
+            self.assertEqual("aws_url", env.base_url)
+
+        # GCP Composer
+        with patch.dict(os.environ, {
+            "COMPOSER_ENVIRONMENT": "gcp_env_name",
+            "COMPOSER_GKE_NAME": "gcp_env_id",
+            "MAJOR_VERSION": "gcp_version",
+            "AIRFLOW__WEBSERVER__BASE_URL": "gcp_url",
+        }):
+            env = AirflowEnv()
+            self.assertEqual("gcp_env_name", env.env_name)
+            self.assertEqual("gcp_env_id", env.env_id)
+            self.assertEqual("gcp_version", env.version)
+            self.assertEqual("gcp_url", env.base_url)
+
+        # Astronomer
+        with patch.dict(os.environ, {
+            "AIRFLOW__WEBSERVER__INSTANCE_NAME": "astro_env_name",
+            "ASTRO_DEPLOYMENT_ID": "astro_env_id",
+            "ASTRONOMER_RUNTIME_VERSION": "astro_version",
+            "AIRFLOW__WEBSERVER__BASE_URL": "astro_url",
+        }):
+            env = AirflowEnv()
+            self.assertEqual("astro_env_name", env.env_name)
+            self.assertEqual("astro_env_id", env.env_id)
+            self.assertEqual("astro_version", env.version)
+            self.assertEqual("astro_url", env.base_url)
+
+        params_env = AirflowEnv(
+            env_name="name",
+            env_id="id",
+            version="1.0",
+            base_url="url"
+        )
+        self.assertEqual("name", params_env.env_name)
+        self.assertEqual("id", params_env.env_id)
+        self.assertEqual("1.0", params_env.version)
+        self.assertEqual("url", params_env.base_url)
+
     def _test_upload_dag_result(
             self,
             success: bool,
             mock_client_upload_result
     ):
         dag_context = self._create_dag_context(success)
         dag: DAG = dag_context["dag"]
```

### Comparing `airflow_mcd-0.1.0/tests/hooks/test_session_hook.py` & `airflow_mcd-0.1.1/tests/hooks/test_session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/tests/operators/test_base_op.py` & `airflow_mcd-0.1.1/tests/operators/test_base_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.1.0/tests/operators/test_circuit_breaker_op.py` & `airflow_mcd-0.1.1/tests/operators/test_circuit_breaker_op.py`

 * *Files identical despite different names*

